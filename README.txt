Instructions and Summary of the Model

1st Step: Install necessary packages as instructed in the initial cells, then import the required libraries.

2nd Step: Update the file paths to match the project folder and the cropped folder within it, which we provided. This step ensures that the images are cropped to remove zero-value pixels before being fed into the model.

3rd Step: Change the paths again, this time to the cropped and 128x128 folders. The model will resize the images to 128x128 pixels and compress them accordingly.

4th Step: Update the path once more, replacing the 128x128 folder path with your designated folder path. The following processes will then take place:

-The code will extract the images to prepare them for the deep learning model.

-Images will be converted to grayscale, as SSPOR operates exclusively with grayscale images.

-The dataset will be split, allocating 80% for training and 20% for testing.

-SSPOR will determine the optimal sensor positions for the chosen number of modes (you can adjust the number of sensors and modes). A visual representation of the selected sensors will be displayed.

-The dataset will be transformed for CNN input. The original colored images will be converted into images with selectively colored sensors in 3 channels (RGB). An example of this transformed CNN input dataset will be shown.

-The CNN architecture will be constructed, and the model will be trained. A graph illustrating the Mean Squared Error (MSE) per epoch will be displayed.

-Finally, a comparison between the CNN input, the CNN output, and the expected result will be presented.

The model has been run with varying numbers of modes and sensors to study the influence of these parameters on the flow field reconstruction.