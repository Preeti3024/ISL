# Indian-sign-language-recognition

Hello, This repository contains python implementation for recognising Indian sign language (ISL) gestures. As there is less research, there is no standard dataset avialable in the web. So, we decided to create my own [dataset](https://drive.google.com/open?id=1keWr7-X8aR4YMotY2m8SlEHlyruDDdVi) of gesture images. ISL dataset have all alphabets (A-Z) and numerics (1-9) with total classes = 35. Each class has 1200 images. ISL gestures are practically hard to recognise as two hands are involved and because of complexity. To classify images, Bag-of-words (bow) model has been implemented with SVM. **70:30** ratio has been used for train and test to split. Using this method, the model gives 99% accuracy approximatly with very less error rate. 

## Run files

Run files in order:<br/>
**Step 1:** (Optional) To create your own Dataset run

>   python image_capture.py

**Step 2:** If you want to use our dataset download from below and extract it in the root directory of the repository.  Then run

>   python imagePreprocessing.py

to preprocess all the images (from raw images to histograms of bovw model) and to classify using SVM.

**Step 3:** To visualise the confusion matrix run the file

>   python visualise.py

Dataset can be downloaded from : https://drive.google.com/open?id=1keWr7-X8aR4YMotY2m8SlEHlyruDDdVi

