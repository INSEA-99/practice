Detection Module including mmdet, mmyolo
============
Usage
------------
### Install
```
conda create --name openmmlab python=3.8 -y
conda activate openmmlab
```
```
conda install pytorch torchvision -c pytorch
pip install -e .
```

### Data Preparation
Prepare COCO format dataset

```
coco_root_dir
    ├── annotations
    │   ├── train.json 
    │   └── val.json
    ├── train 
    │   ├── image1.jpg 
    │   ├── image2.jpg
    │        '''
    └── val
        ├── image3.jpg 
        ├── image4.jpg
             '''

```
you can use 'labelme_to_coco.py' to convert labelme format to coco format.
```
python labelme_to_coco.py root_dir classes --save_dir --split_ratio
python labelme_to_coco.py './root_dir' 'class1' 'class2' 'class3'
```
root_dir must have labelme json files and images.  
```
root_dir
    ├── image1.jpg
    ├── image1.json
    ├── image2.jpg
    ├── image2.json
          '''
```



