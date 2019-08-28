# facerecogntion 
This was my project done in july -ocotber 2018
This project basically trains the data by tha images saved by webcam and after training the data it runs the program which recognizes the face and shows the name at the bottom right of the face .
This was my project report 
 
 -----------------------------------------------------------------------------------------------------------------------------------------
 
                                                          ABSTRACT 
The growing interest in computer vision of the past decade. Fueled by the steady doubling rate of computing power every 13 months, face detection and recognition has transcended from an esoteric to a popular area of research in computer vision and one of the better and successful applications of image analysis and algorithm based understanding. Because of the intrinsic nature of the problem, computer vision is not only a computer science area of research, but also the object of neuroscientific and psychological studies, mainly because of the general opinion that advances in computer image processing and understanding research will provide insights into how our brain work and vice versa. Because of general curiosity and interest in the matter, I proposed to create an application that would allow user access to a particular machine based on an in-depth analysis of a person’s facial features.  
 
 
Identifying a person with an image has been popularized through the mass media. However, it is less robust to fingerprint or retina scanning. This report describes the face detection and recognition mini-project undertaken at Maharaja Surajmal Institute of Technology. It reports the technologies available in the OpenComputer-Vision (OpenCV) library and methodology to implement them using Python.  
 
 
For face detection, Haar-Cascades were used and for face recognition Eigenfaces, Fisherfaces and Local binary pattern histograms were used. The methodology is described including flow charts for each stage of the system. Next, the results are shown including plots and screen-shots followed by a discussion of encountered challenges. The report is concluded with the authors’ opinion on the project and possible applications. 


                                           ABBREVIATIONS  AND ACRONYMs
 
 
 
 
OpenCV     Open Source Computer Vision 
LBPH       Local Binary Pattern Histogram 
LDA        Linear Discriminant Analysis 
PCA        Principal Component Analysis 
RGB        Red Green Blue 
Scrn       Screen Shot 
FIG        Figure 





                                                           Chapter-1 INTRODUCTION 
1.1 About the Project 
The following document is a report on the mini project for Face Recognition. It involved building a system for face detection and face recognition using several classifiers available in the open computer vision library(OpenCV). Face recognition is a noninvasive identification system and faster than other systems since multiple faces can be analyzed at the same time. The difference between face detection and identification is, face detection is to identify a face from an image and locate the face. Face recognition is making the decision ”whose face is it ? ”, using an image database. In this project both are accomplished using different techniques and are described below. The report begins with a brief history of face recognition. This is followed by the explanation of HAARcascades, Eigenface, Fisherface and Local binary pattern histogram (LBPH) algorithms. Next, the methodology and the results of the project are described. A discussion regarding the challenges and the resolutions are described. Finally, a conclusion is provided on the pros and cons of each algorithm and possible implementations 


                                                    Chapter-2 HISTORY OF FACE RECOGNITION  

2.1 History 

Face recognition began as early as 1977 with the first automated system being introduced By Kanade using a feature vector of human faces [1]. In 1983, Sirovich and Kirby introduced the principal component analysis(PCA) for feature extraction [2]. Using PCA, Turk and Pentland Eigenface was developed in 1991 and is considered a major milestone in technology [3]. Local binary pattern analysis for texture recognition was introduced in 1994 and is improved upon for facial recognition later by incorporating Histograms(LBPH) [4], [5]. In 1996 Fisherface was developed using Linear discriminant analysis (LDA) for dimensional reduction and can identify faces in different illumination conditions, which was an issue in Eigenface method [6]. Viola and Jones introduced a face detection technique using HAAR cascades and ADABoost [7]. In 2007, A face recognition technique was developed by Naruniec and Skarbek using Gabor Jets that are similar to mammalian eyes [8], [9]. In This project, HAAR cascades are used for face detection and Eigenface, Fisherface and LBPH are used for face recognition.  

                                            Chapter-3  FACE DETECTION USING HAAR – CASCADES 
3.1 Introduction to Haar-Cascades 

A Haar wavelet is a mathematical  fiction that produces square-shaped waves with a beginning and an end and used to create box shaped pattern   to recognize signals with sudden transformations. An example is shown in figure 3.1. By combining several wavelets , a cascade  can be created that can identify edges, lines and circles with different color intensities. These sets are used in Viola Jones face detection technique in 2001 and since then more patterns are introduced  [10] for object detection as shown in figure 3.1. To analyse an image using Haar cascades, a scale is selected smaller than the target image. It is then placed on the image, and the average of the values of pixels in each section is taken. If the difference between two values pass a given threshold, it is considered a match. Face detection on a human  face is performed by matching a combination of different Haar-likefeatures. For example, forehead, eyebrows and eyes contrast as well as the nose with eyes as shown below in figure A single classifier is not accurate enough. Several classifiers are combined as to provide an accurate face detection system as shown in the block diagram below in figure 3.3. 
 
 
                                                           RESULTS
The collected images are shown below. Each face has 10 images. Three applications were written to iterate through the parameters of each algorithm. On each iteration, the algorithm is trained using different parameters and tested against a photo. The resulting data is plotted at the after finishing the tests. 
The applications are : • TestDataCollector EigenFace.py • TestDataCollector FisherFace.py  • TestDataCollector LBPH.py. 



                                                            Conclusion
This paper describes the mini-project for visual perception and autonomy module. Next, it explains the technologies used in the project and the methodology used. Finally, it shows the results, discuss the challenges and how they were resolved followed by a discussion. Using Haar-cascades for face detection worked extremely well even when subjects wore spectacles. Real time video speed was satisfactory as well devoid of noticeable frame lag. Considering all factors, LBPH combined with Haar-cascades can be implemented as a cost effective face recognition platform. An example is a system to identify known troublemakers in a mall or 18 a supermarket to provide the owner a warning to keep him alert or for automatic attendance taking in a class
