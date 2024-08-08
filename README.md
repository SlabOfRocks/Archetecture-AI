# Archetecture-AI
My AI can look at the image of a building and tell you from what time period it is from, it works on modern, postmodern, ancient and more recent but non-Modern buildings. This AI will allow people less experienced in buildings to be able to figure out how old a building might be without much in-depth research. This can help tourists, agents surveying buildings or just curious people. 


# hi
This AI uses architectural styles to identify buildings and recognize what time period it is from. It runs using a re-trained resnet-18 convolutional model allowing it to identify shapes in buildings. A Resnet-18 model uses multiple layers in order to break down an image using different filters and skipping over steps. It was trained using a dataset of architectural styles re-sorted using code into time periods. The data was received from kaggle, a dataset website. The photos contained in the dataset consist of buildings sorted into subfolders of architectural styles. Although it is still confused about some buildings now, with more time, training and data, this AI will be able to fully recognize architectural styles.
