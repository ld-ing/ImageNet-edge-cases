# Keras-ImageNet  
Keras implementation to test pre-trained models on ImageNet, as well as interactively show and explore failure cases.  
Li Ding  
Oct. 20, 2017  

### Overview  
- `imgnet-val-resnet50.py` - load the pre-trained ResNet-50 and evaluate on ILSVRC'12 validation set, save the prediction result.  
- `imgnet-val-explore.ipynb` - use the prediction to interactively explore failure cases in Jupyter Notebook.  

### Quick Start  
- dependencies: `Python 2.7 + tensorflow, keras, xmltodict, Queue, threading, tqdm, cv2`  
- set data path: enter a folder path in both files, e.g. `'/imgnet'` that has following structure:  
  ```
  /imgnet  
  .../ILSVRC2012_img_val/ (ILSVRC'12 validation images, 50,000 items, totalling 6.7GB)  
  .../val/ (ILSVRC'12 validation annotations, 50,000 .xml files, totalling 31.2 MB)  
  .../val_prob.csv (optional, the prediction created by imgnet-val-resnet50.py)  
  ```  
- run `imgnet-val-resnet50.py` to obtain the result `val_prob.csv`.  
- in terminal, `jupyter notebook` to start jupyter, load `imgnet-val-explore.ipynb`, run and explore.  

![alt text](https://github.com/Zephyr-D/keras-imagenet/blob/master/demo.png "Demo")

