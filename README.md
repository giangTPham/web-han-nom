Code from [here] (https://github.com/MhLiao/DB).
```
pip install -r requirement.txt
cd \assets\ops\dcn 
python setup.py build_ext --inplace
cd ..
cd ..
cd ..
python app.py
```
Open a web browser, go to `http://localhost:5000`
Upload `/test/LienPhai-2484.jpg` and wait...

Only want to run a sample?
```
CUDA_VISIBLE_DEVICES=0 python demo.py experiments/seg_detector/td500_resnet18_deform_thre.yaml --image_path test/sample_1.jpg --resume weights/final --box_thresh 0.6
```
Finally watch your results in demo_result folder
