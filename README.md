


## To Reproduce Our Results on THUMOS14
**Download Features and Annotations**
* Download *thumos.tar.gz* (`md5sum 375f76ffbf7447af1035e694971ec9b2`) from [this Box link](https://uwmadison.box.com/s/glpuxadymf3gd01m1cj6g5c3bn39qbgr) or [this Google Drive link](https://drive.google.com/file/d/1zt2eoldshf99vJMDuu8jqxda55dCyhZP/view?usp=sharing) or [this BaiduYun link](https://pan.baidu.com/s/1TgS91LVV-vzFTgIHl1AEGA?pwd=74eh).
* The file includes I3D features, action annotations in json format (similar to ActivityNet annotation format), and external classification scores.

**Details**: The features are extracted from two-stream I3D models pretrained on Kinetics using clips of `16 frames` at the video frame rate (`~30 fps`) and a stride of `4 frames`. This gives one feature vector per `4/30 ~= 0.1333` seconds.

## To Reproduce Our Results on ActivityNet 1.3
**Download Features and Annotations**
* Download *anet_1.3.tar.gz* (`md5sum c415f50120b9425ee1ede9ac3ce11203`) from [this Box link](https://uwmadison.box.com/s/aisdoymowukc99zoc7gpqegxbb4whikx) or [this Google Drive Link](https://drive.google.com/file/d/1VW8px1Nz9A17i0wMVUfxh6YsPCLVqL-S/view?usp=sharing) or [this BaiduYun Link](https://pan.baidu.com/s/1tw5W8B5YqDvfl-mrlWQvnQ?pwd=xuit).
* The file includes TSP features, action annotations in json format (similar to ActivityNet annotation format), and external classification scores.

**Details**: The features are extracted from the R(2+1)D-34 model pretrained with TSP on ActivityNet using clips of `16 frames` at a frame rate of `15 fps` and a stride of `16 frames` (*i.e.,* **non-overlapping** clips). This gives one feature vector per `16/15 ~= 1.067` seconds. The features are converted into numpy files for our code.



**[Optional] Reproducing Our Results with I3D Features**

* Download *anet_1.3_i3d.tar.gz* (`md5sum e649425954e0123401650312dd0d56a7`) from [this Google Drive Link](https://drive.google.com/file/d/16239kUT2Z-j6S6PXIT1b_31OJi35QW_o/view?usp=sharing).

**Details**: The features are extracted from the I3D model pretrained on Kinetics using clips of `16 frames` at a frame rate of `25 fps` and a stride of `16 frames`. This gives one feature vector per `16/25 = 0.64` seconds. The features are converted into numpy files for our code.


## To Reproduce Our Results on EPIC Kitchens 100
**Download Features and Annotations**
* Download *epic_kitchens.tar.gz* (`md5sum add9803756afd9a023bc9a9c547e0229`) from [this Box link](https://uwmadison.box.com/s/vdha47qnce6jhqktz9g4mq1gc40w82yj) or [this Google Drive Link](https://drive.google.com/file/d/1Z4U_dLuu6_cV5NBIrSzsSDOOj2Uar85X/view?usp=sharing) or [this BaiduYun Link](https://pan.baidu.com/s/15tOdX6Yp4AJ9lFGjbQ8dgg?pwd=f3tx).
* The file includes SlowFast features as well as action annotations in json format (similar to ActivityNet annotation format).

**Details**: The features are extracted from the SlowFast model pretrained on the training set of EPIC Kitchens 100 (action classification) using clips of `32 frames` at a frame rate of `30 fps` and a stride of `16 frames`. This gives one feature vector per `16/30 ~= 0.5333` seconds.
