# Handwritten-OCR

Problem Statement: To recognize handwritten text from forms (with grids, e.g.- a bank form) and export as CSV file.

Collected data by scanning bank like forms. Used OpenCV to detect contours, Noise removal using Gaussian blur, dilate function to increase contour detection accuracy.

Total Classes- 47 ( 10 digits , 26 Capital alphabets , 11 special characters  <b> space , . / () + - & @ : </b>

Model - Used Renet as final model and made custom rules over the model,  which forces model to predict characters as per the form characteristics on row level. e.g. – In mobile number model will can predict only digits and in name column model can predict alphabets only. So, able to reduce errors in between classes where the model was getting confuse like ‘0’ and ‘O’, ‘1, and ‘I’ etc.

Working - Please copy the file 2.jpg from Data Sample folder. Model used for prediction is in below link https://drive.google.com/open?id=1iCWepWM51vyQxEfnOfj4_lfmT7j3y64a with the name of 'model_letters_digits_space_sc_89_r2.h5'. 

Now,
In the model code folder run 'One Tap Updater.ipynb'  file and once GUI  open, copy the image file path you want to convert jpg to excel. If multi images choose option 'All at one time' in GUI. It will be converted in 15-20 secs. Please check workflow image for more clarity and also exe file documentaion in main folder.

One executbale file for windows can be found in below link:-
https://drive.google.com/open?id=1iCWepWM51vyQxEfnOfj4_lfmT7j3y64a

Note: - The program is for specifed type of form. If some changes in form struture then some modification will be reuiqred as per the form struture to detect all contours.
