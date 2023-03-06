# Implementasi Algoritma YOLOv5 Pada Pengenalan WajahSecara Real-Time

## Proses Preprocessing data
1. Latih algoritma YOLOv5 dengan kumpulan data wajah supaya bisa mendeteksi wajah seseorang. Kumpulan data wajah bisa didapatkan di internet seperti dataset WIDERFACE (http://shuoyang1213.me/WIDERFACE/) atau dataset CelebA (http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html). Sebelum melatihnya, convert dataset ke dalam format YOLO.
2. Kumpulkan data-data wajah orang yang ingin dilakukan pengenalan dan dibuat dalam 1 folder sesuai dengan nama tiap-tiap wajah.
3. Lakukan preprocessing pada data wajah orang yang telah dikumpulkan sebelum dilakukan ekstraksi fitur. (Note: Ekstraksi fitur Facenet mengharuskan ukuran gambar file sebesar 160x160 pixels)
4. Lakukan ekstraksi fitur menggunakan algortima FACENET dengan data wajah orang yang sudah dilakukan preprocessing. dengan menjalankan file embeddings.py. 
5. Kemudian klasifikasikan data wajah yang sudah di ekstraksi dengan menjalankan classificationSVM.py

## Cara Menjalankan Program
```bash
$ python recognition/test.py --source 0
```

## Requirements

Python 3.7 or later with all `requirements.txt` dependencies installed, including `torch >= 1.5`. To install run:
```bash
$ pip install -U -r requirements.txt
```

## Source
YOLOv5:(https://github.com/ultralytics/yolov5)<br>
FACENET:(https://github.com/davidsandberg/facenet)<br>
Program:(https://blog.csdn.net/ninesky110/article/details/84844307) <br>
Dataset:(http://shuoyang1213.me/WIDERFACE)
