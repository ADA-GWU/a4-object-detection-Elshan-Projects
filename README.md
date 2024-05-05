* The notebook containing my solution: ___Assignment_5_NB.ipynb___
* The image used for the experiments is at: ___Original_Images/Image_1.jpeg___
* Dependencies: ___pip install opencv-python numpy easyocr matplotlib___

# Border Detection
Border detection is done by initially detecting the edges with opencv's Canny and then a rectangular contour is recognized to be displayed on top of the original image.
# Perpective transform
Perspective transform is also done with opencv by transforming the rectangular contour from the ___"Border Detection"___ stage into 4 corner points. The resulting image is saved in the folder named ___"Results_Folder"___ under the name ___"image_name"+"_Perspective"___ and displayed with matplotlib.
# Text Recognition
Text Recognition was carried out with MSER where the detected text was highlighted with red. The resulting image is saved in the folder named ___"Results_Folder"___ under the name ***"image_name"+"_MSER"*** and displayed with matplotlib.
# Image to Text conversion With a Pre-trained Model
A pre-trained CRNN model was loaded via the "easyocr" library which extracted the text from the ___"highlighted_image"___ array from the ___"Text Recognition"___ stage to be printed and saved in the ___"Results_Folder"___ under the name ___"image_name"+"Text"___ in ___txt___ format.
