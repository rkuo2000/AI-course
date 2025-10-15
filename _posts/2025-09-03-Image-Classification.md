---
layout: post # 指定文章佈局，通常是 post
title: Image Classification
date: 2025-09-03 08:00:00 +0800 # 發表日期和時間 (請根據您當前的時區調整 +0800 代表 UTC+8)
categories: [Lecture] # 文章分類，您可以自訂
tags: [CNN] # 文章標籤，您可以自訂
description: Image Classification (影像分類)
mathjax: false # 如果這篇文章不需要顯示數學公式，請設false
comments: false # 如果這篇文章需要啟用評論，請設為 true

---
## Datasets

### [PASCAL VOC (Visual Ojbect Classes)](http://host.robots.ox.ac.uk/pascal/VOC/)
VOC2007 train/val/test 9,963張標註圖片，有24,640個標註物件<br> 
VOC2012 train/val/test11,530張標註圖片，有27,450個ROI 標註物件<br>
![](https://github.com/ultralytics/docs/releases/download/0/mosaiced-voc-dataset-sample.avif)
**20** classes:
* Person: person
* Animal: bird, cat, cow, dog, horse, sheep
* Vehicle: aeroplane, bicycle, boat, bus, car, motorbike, train
* Indoor: bottle, chair, dining table, potted plant, sofa, tv/monitor

---
### [COCO Dataset](https://cocodataset.org/)
![](https://cocodataset.org/images/coco-examples.jpg)
* Object segmentation
* Recognition in context
* Superpixel stuff segmentation
* 330K images (>200K labeled)
* 1.5 million object instances
* **80** object categories
* 91 stuff categories
* 5 captions per image
* 250,000 people with keypoints

---
### [ImageNet](http://www.image-net.org/)
This dataset spans **1000 object** classes and contains 1,281,167 training images, 50,000 validation images and 100,000 test images. This subset is available on [Kaggle](https://www.kaggle.com/competitions/imagenet-object-localization-challenge/data).<br>
![](https://miro.medium.com/max/700/1*IlzW43-NtJrwqtt5Xy3ISA.jpeg)

---
## Applications

### CIFAR-10
**Dataset:** [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html)<br>
The CIFAR-10 dataset consists of 60000 32x32 colour images in 10 classes, with 6000 images per class. There are 50000 training images and 10000 test images.<br>
![](https://github.com/rkuo2000/AI-course/blob/main/assets/images/CIFAR-10.png?raw=true)

**Kaggle:** [rkuo2000/cifar10-cnn](https://www.kaggle.com/rkuo2000/cifar10-cnn)<br>

---
### Traffic Sign Classifier (交通號誌辨識)
**Dataset:** [German Traffic Sign Recognition Benchmark (GTSRB)](https://benchmark.ini.rub.de/gtsrb_news.html)<br>
34 traffic signs, 39209 training images, 12630 test images<br>
![](https://assets-global.website-files.com/5d7b77b063a9066d83e1209c/61e9ce225148f6519be6c034_GTSRB-0000000633-9ce3c5f6_Dki5Rsf.jpeg)

**Kaggle:** [rkuo2000/GTSRB-CNN](https://www.kaggle.com/rkuo2000/gtsrb-cnn)<br>

---
### Emotion Detection (情緒偵測)
**Dataset:** [FER-2013 (Facial Expression Recognition)](https://www.kaggle.com/datasets/msambare/fer2013)<br>
![](https://www.researchgate.net/profile/Chaudhary-Aqdus/publication/349055345/figure/fig3/AS:987834383085568@1612529478973/FER-2013-sample-images-for-facial-emotion-recognition.jpg)

7 facial expression, 28709 training images, 7178 test images<br>
labels = ["angry", "disgusted", "fearful", "happy", "neutral", "sad", "surprised"]<br>
**Kaggle:** [rkuo2000/FER2013-CNN](https://www.kaggle.com/rkuo2000/fer2013-cnn)<br>

---
### Pneumonia Detection (肺炎偵測)
**Dataset:** [https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia)<br>
![](https://raw.githubusercontent.com/anjanatiha/Pneumonia-Detection-from-Chest-X-Ray-Images-with-Deep-Learning/master/demo/sample/sample.png)

**Kaggle:** [rkuo2000/Pneumonia-CNN](https://www.kaggle.com/rkuo2000/pneumonia-cnn)<br>

---
### COVID19 Detection (新冠肺炎偵測)
**Dataset:** [https://www.kaggle.com/bachrr/covid-chest-xray](https://www.kaggle.com/bachrr/covid-chest-xray)<br>
![](https://i.imgur.com/jZqpV51.png)

**Kaggle:** [rkuo2000/COVID19-VGG16](https://www.kaggle.com/rkuo2000/covid19-vgg16)<br>

---
### FaceMask Classification (人臉口罩辨識)
**Dataset:** [Face Mask ~12K Images dataset](https://www.kaggle.com/datasets/ashishjangra27/face-mask-12k-images-dataset)<br>
![](https://github.com/rkuo2000/AI-course/blob/main/assets/images/facemask_12k_dataset.png?raw=true)

**Kaggle:** [rkuo2000/Facemask-CNN](https://www.kaggle.com/rkuo2000/facemask-cnn)<br>

---
### Garbage Classification (垃圾分類)
**Dataset:** https://www.kaggle.com/asdasdasasdas/garbage-classification (42MB)<br>
6 categories : cardboard(403), glass(501), metal(410), paper (594), plastic(482), trash(137)<br>
<img widtih="50%" height="50%" src="https://miro.medium.com/max/2920/1*mJipx8yxeI_JW36jDAuM9A.png">

**Kaggle:** [rkuo2000/Garbage-CNN](https://www.kaggle.com/rkuo2000/garbage-cnn)<br>

---
### Food Classification  (食物分類)
**Dataset:** [Food-11](https://mmspg.epfl.ch/downloads/food-image-datasets/)<br>
![](https://929687.smushcdn.com/2633864/wp-content/uploads/2019/06/fine_tuning_keras_food11.jpg?lossy=1&strip=1&webp=1)
The dataset consists of 16,643 images belonging to 11 major food categories:<br>
* Bread (1724 images)
* Dairy product (721 images)
* Dessert (2,500 images)
* Egg (1,648 images)
* Fried food (1,461images)
* Meat (2,206 images)
* Noodles/pasta (734 images)
* Rice (472 images)
* Seafood (1,505 images)
* Soup (2,500 images)
* Vegetable/fruit (1,172 images)

**Kaggle:** [rkuo2000/Food11-Classification](https://www.kaggle.com/rkuo2000/food11-classification)<br>

---
### Mango Classification (芒果分類)
**Dataset:** [台灣高經濟作物 - 愛文芒果影像辨識正式賽](https://aidea-web.tw/aicup_mango)<br>
**Kaggle:** [rkuo2000/Mango-Classification](https://www.kaggle.com/rkuo2000/mango-classification), [rkuo2000/mango-efficientnet](https://www.kaggle.com/rkuo2000/mango-efficientnet) <br>

---
## Transer Learning

### Birds Classification (鳥類分類)
**Dataset:** [https://www.kaggle.com/rkuo2000/birds2](https://www.kaggle.com/rkuo2000/birds2)<br>
用Google搜尋照片, 下載各20/30張照片，放入資料夾birds後，壓縮成birds.zip, 再上傳Kaggle.com/datasets<br>
![](https://github.com/rkuo2000/AI-course/blob/main/assets/images/birds_dataset.png?raw=true)

**Kaggle:** [rkuo2000/Birds-Classification](https://www.kaggle.com/rkuo2000/birds-classification)<br>

---
### Animes Classification (卡通人物分類)
**Dataset:** [https://www.kaggle.com/datasets/rkuo2000/animes](https://www.kaggle.com/datasets/rkuo2000/animes)<br>
用Google搜尋照片, 下載卡通人物各約20/30張照片，放入資料夾animes後，壓縮成animes.zip, 再上傳Kaggle.com/datasets<br>
![](https://github.com/rkuo2000/AI-course/blob/main/assets/images/animes_dataset.png?raw=true)

**Kaggle:** [rkuo2000/Anime-Classification](https://www.kaggle.com/rkuo2000/anime-classification)<br>

---
### Worms Classification(害蟲分類)
**Dataset:** [worms4](https://www.kaggle.com/datasets/rkuo2000/worms4)<br>
用Google搜尋照片, 下載各20/30張照片，放入資料夾worms後，壓縮成worms.zip, 再上傳Kaggle.com/datasets<br>
![](https://github.com/rkuo2000/AI-course/blob/main/assets/images/worms4_dataset.png?raw=true)

**Kaggle:** [rkuo2000/Worms-Classification](https://www.kaggle.com/rkuo2000/worms-classification)<br>

---
### Railway Track Fault Detection (鐵軌故障偵測)
**Dataset:** [Railway Track Fault Detection](https://www.kaggle.com/salmaneunus/railway-track-fault-detection)<br>
**Kaggle:** [rkuo2000/Railtrack-ResNet50v2](https://www.kaggle.com/code/rkuo2000/railtrack-resnet50v2), [rkuo2000/railtrack-efficientnet](https://www.kaggle.com/code/rkuo2000/railtrack-efficientnet)<br>

---
### Skin Lesion Classification (皮膚病變分類)
**Dataset:** [Skin Cancer MNIST: HAM10000](https://www.kaggle.com/kmader/skin-cancer-mnist-ham10000)<br>
<img width="50%" height="50%" src="https://user-images.githubusercontent.com/50828923/148700267-6a94f2ca-d914-439d-bf11-f0843cb4d3cc.png">

7 types of lesions : (picture = 600x450)<br>
* Actinic Keratoses (光化角化病)
* Basal Cell Carcinoma (基底細胞癌)
* Benign Keratosis (良性角化病)
* Dermatofibroma (皮膚纖維瘤)
* Malignant Melanoma (惡性黑色素瘤)
* Melanocytic Nevi (黑素細胞痣)
* Vascular Lesions (血管病變)
<br>
**Kaggle:** [rkuo2000/Skin-Lesion-Classification](https://www.kaggle.com/code/rkuo2000/skin-lesion-classification)<br>

<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*

