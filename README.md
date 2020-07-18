# Face-Recognition-using-FaceNet
Thank you davidsandberg for inspiring me tp write this program. you can check this github. https://github.com/davidsandberg/facenet
 you can download pre-trained model from this link: https://drive.google.com/file/d/1R77HmFADxe87GmoLwzfgMu_HY0IhcyBz/view
##Structure of file:

#Sample data
##    |__persion1:
##         |__ image1.jpg
##         |__ image2/jpg
##         |__...
##    |__persion2:
##      |__ image1.jpg
##      |__ image2/jpg
##      |__   
##   ...
test data
How does it work:
+ Load Sample data using MTCNN to detect face and align image. After that save output_image to new folder
+ Load image from folder from above step and Pass it through the model, output is embedding feature(including 256 dimension) and name. Save it to new folder
+ Load test data using MTCNN to detect face and align image. After that save output_image to new folder
+ Load image from folder from above step and Pass it through the model, after that caculate distance between test image and embedding feature of Sample data.
 the object that have The smallest distance is target
