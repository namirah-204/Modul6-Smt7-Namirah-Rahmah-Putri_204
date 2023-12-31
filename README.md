# UAP-Smt7-Namirah-Rahmah-Putri_202010370311204

<!-- PROJECT LOGO -->
<br />
<div align="center">
    <img src="picture/logo umm.png" alt="Logo" width="180" height="180">

<h1 align="center">Rock, Paper, Scissors Prediction</h1>
  <p align="center">
    Project ini berfokus untuk memprediksi gambar (Rock, Paper, Scissors) dengan model VGG19
  </p>
</div>

## Author : Namirah Rahmah Putri_202010370311204 

## DATASET 
Dataset yang digunakan dalam project ini berisi total 2520 gambar dengan pembagian setiap kelas berjumlah sama : 840 gambar (dibagi secara rata). [Link dataset dapat diakses di sini.](https://drive.google.com/drive/folders/1rpn0itTAOCvTuLxdJnnhGDH5OxkJGNCA?usp=drive_link)

<div>
    <img src="picture/dataset.jpeg" alt="dataset" width="75%">
</div>

## PREPROCESSING 
Dataset ini terbagi menjadi 3 set (train:80, test:10, validation:10)
```python
splitfolders.ratio("Dataset/Images/rps/", output="Dataset/Images/rps_split",
    seed=1337, ratio=(.8, .1, .1), group_prefix=None, move=False)
```


