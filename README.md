# computervision
Requirements:The code is compatible with python 3.0+(Ubuntu 18.04)
Running Handle_case_c(opencv-text-recognition -case 3)  folder  in source code  follow below instructions.
1.OpenCv
2.Numpy
3.argparse
4.Tesseract
project structure should be like this:
Be sure to go to main folder using cd command after getting below structure then only you have to run.




![1](https://user-images.githubusercontent.com/38165350/57343437-07509a00-7161-11e9-8947-c01918e2fa5b.jpg)

images/ : A directory containing sone test images containing scene text. We will attempt OpenCV OCR with each of these images. 
    • frozen_east_text_detection.pb : The EAST text detector. This CNN  is pre-trained for text detection and ready to go. I did not train this model — it is provided with OpenCV; I’ve also included it in the “Downloads” for your convenience. 
    • text_recognition.py : Our script for OCR — we’ll review this script line by line. The script utilizes the EAST text detector to find regions of text in the image and then takes advantage of Tesseract v4 for recognition. 
After that run this command to execute the code:
python text_recognition.py --east frozen_east_text_detection.pb \
   --image images/image7_for_ocr.jpg
Then output will be like this:
![2](https://user-images.githubusercontent.com/38165350/57343602-9f4e8380-7161-11e9-84d0-dbab31a5fd64.jpg)
Press Enter to continue to detect other cells text like this :
![3](https://user-images.githubusercontent.com/38165350/57343610-a5dcfb00-7161-11e9-8274-780af849bf99.jpg)
