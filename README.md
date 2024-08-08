# Archetecture-AI
My AI can look at the image of a building and tell you from what time period it is from, it works on modern, postmodern, ancient and more recent but non-Modern buildings. This AI will allow people less experienced in buildings to be able to figure out how old a building might be without much in-depth research. This can help tourists, agents surveying buildings or just curious people. 


# The Algorithm
This AI uses architectural styles to identify buildings and recognize what time period it is from. It runs using a re-trained resnet-18 convolutional model allowing it to identify shapes in buildings. A Resnet-18 model uses multiple layers in order to break down an image using different filters and skipping over steps. It was trained using a dataset of architectural styles re-sorted using code into time periods. The data was received from kaggle, a dataset website. The photos contained in the dataset consist of buildings sorted into subfolders of architectural styles. Although it is still confused about some buildings now, with more time, training and data, this AI will be able to fully recognize architectural styles.


# Downloading instructions
1. Download the Jetson-Inference library and Python3 and make sure you have a Jetson Nano.
2. Activate the Nano and connect it to your computer.
3. Create a folder with any name in your Nano.
4. Go to the ResNet-18 model and download into the folder you just created.
>   https://drive.google.com/file/d/1i0aO-qSefy1qC_GNcGZNhAStCvjSWuyP/view?usp=sharing 
5. Also download the classification labels to the same folder.
 >  https://drive.google.com/file/d/1NIkvHchZjkA2HPYxHyTlDC6G8mFN-Rfy/view?usp=sharing
6. Create a subfolder called images.
7. Download any images you want to use into that folder.
8. Go back to the bigger folder to run this in the command terminal:
 >  $ imagenet.py --model=resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=labels.txt “images/NAME_OF_FILE.jpg” NAME_OF_OUTPUT.jpg


# Demo Video
>https://drive.google.com/file/d/1Z8oNPgMVFecpDokgAwoqX4JYYL9iS5LZ/view?usp=sharing
