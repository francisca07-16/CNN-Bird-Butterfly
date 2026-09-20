# CNN Bird & Butterfly Image Classification

## Pengenalan

Projek ini membangunkan sistem kecerdasan buatan (AI) menggunakan Convolutional Neural Network (CNN) untuk mengklasifikasikan imej kepada dua kategori, iaitu Bird dan Butterfly.

Model dibangunkan menggunakan Python dan PyTorch melalui platform Google Colab.

## Dataset

Dataset mengandungi dua kelas imej:

* Bird
* Butterfly

Dataset dibahagikan kepada dua bahagian:

* `train` – digunakan untuk melatih model.
* `test` – digunakan untuk menguji prestasi model.

## Preprocessing

Imej diproses menggunakan beberapa langkah sebelum digunakan dalam model CNN:

* Resize kepada 64 × 64 piksel.
* Random Horizontal Flip untuk data training.
* Menukarkan imej kepada tensor menggunakan `ToTensor()`.

## Model CNN

Model `BirdButterflyCNN` mempunyai tiga lapisan convolution yang digunakan untuk mengekstrak ciri daripada imej.

Komponen utama model:

* Convolutional Layer
* ReLU Activation
* Max Pooling
* Flatten
* Fully Connected Layer
* Output untuk dua kelas

## Training

Model dilatih menggunakan:

* Loss Function: CrossEntropyLoss
* Optimizer: Adam
* Learning Rate: 0.001
* Epochs: 3

## Hyperparameter Tuning

Hyperparameter tuning dilakukan dengan membandingkan dua nilai learning rate:

* 0.001
* 0.01

Perbandingan dibuat berdasarkan Test Accuracy yang diperoleh bagi setiap learning rate.

## Deployment

Model digunakan untuk membuat prediction terhadap imej baharu yang dimuat naik melalui Google Colab.

## Teknologi Digunakan

* Python
* PyTorch
* Google Colab
* Git
* GitHub

## Fail Projek

`CNN_Bird_Butterfly.ipynb` mengandungi keseluruhan kod pembangunan model CNN, termasuk preprocessing, training, testing, hyperparameter tuning dan deployment.
Development branch digunakan untuk proses pembangunan dan pengurusan perubahan projek.
