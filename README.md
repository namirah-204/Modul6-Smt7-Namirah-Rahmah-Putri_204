# UAP-Smt7-Namirah-Rahmah-Putri_202010370311204

<!-- PROJECT LOGO -->
<br />
<div align="center">
    <img src="picture/logo umm.png" alt="Logo" width="180" height="180">

<h1 align="center">Rock, Paper, Scissors Prediction</h1>
  <p align="center">
    Project ini berfokus untuk memprediksi gambar (Rock, Paper, Scissors) dengan pre-trained model VGG-16
  </p>
</div>

## Author : Namirah Rahmah Putri_202010370311204 

## DATASET 
Dataset yang digunakan dalam project ini berisi total 2520 gambar dengan pembagian setiap kelas berjumlah sama : 840 gambar (dibagi secara rata). [Link dataset dapat diakses di sini.](https://drive.google.com/drive/folders/1rpn0itTAOCvTuLxdJnnhGDH5OxkJGNCA?usp=drive_link)

<div>
    <img src="picture/dataset.jpeg" alt="dataset" width="75%">
</div>

## PREPROCESSING 
Dataset ini terbagi menjadi 3 set :
- train : 80
- test : 10
- validation : 10
  
```python
splitfolders.ratio("Dataset/Images/rps/", output="Dataset/Images/rps_split",
    seed=1337, ratio=(.8, .1, .1), group_prefix=None, move=False)
```

Selanjutnya, data ini diaugmentasi dengan parameter :
- rotation_range=30
- shear_range=0.2
- zoom_range=0.025
- horizontal_flip=True
- vertical_flip=True
- width_shift_range=0.05
- height_shift_range=0.05
- brightness_range=(1,1.1)

<div>
    <img src="picture/augmentasi.png" alt="dataset yang diaugmentasi" width="75%">
</div>

## DEEP LEARNING MODEL 
Project ini menggunakan training VGG-16. VGG-16 adalah sebuah arsitektur deep convolutional neural network yang terdiri atas 16 layer dan merupakan salah satu arsitektur paling awal yang digunakan dalam transfer learning.

<div>
    <img src="picture/Arsitektur Model VGG-16.png" alt="arsitektur vgg-16" width="75%">
</div>

### MODEL TRAINING
|   Training and Validation accuracy | Training and Validation loss |
| ------------- | ------------- |
| ![](picture/accuracy.png)  | ![](picture/loss.png)  |

## MODEL EVALUATION 
Setelah proses training, model ini akan di evaluasi dan didapatkan hasil akurasi sebanyak 99 % 

<div>
    <img src="picture/eval.png" alt="model evaluation" width="75%">
</div>

## TAMPILAN WEBSITE 
1. Tampilan awal
<div>
    <img src="picture/1.png" alt="web" width="75%">
</div>

2. Tampilan setelah menginputkan gambar
<div>
    <img src="picture/2.png" alt="web" width="75%">
</div>


3. Tampilan ketika selesai memprediksi untuk menampilkan akurasi
<div>
    <img src="picture/3.png" alt="web" width="75%">
</div>


