# Handwritten-OCR

Problem Statement: To recognize handwritten text from forms (with grids, e.g.- a bank form) and export as CSV file.

Collected data by scanning bank like forms. Used OpenCV to detect contours, Noise removal using Gaussian blur, dilate function to increase contour detection accuracy.

Total Classes- 47 ( 10 digits , 26 Capital alphabets , 11 special characters  <b> space , . / () + - & @ : </b>

Model - Used Renet as final model and made custom rules over the mode,  which forces model to predict characters as per the form characteristics on row level. e.g. – In mobile number model will can predict only digits and in name column model can predict alphabets only. So, we able to reduce errors in between classes where the model was getting confuse like ‘0’ and ‘O’, ‘1, and ‘I’ etc.
