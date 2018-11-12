# Kaggle Project

<h4>01/11/2018 (Charles)</h4> </n>
I created the Github, added the raw data and example submission.

<h4>12/11/2018 (Charles)</h4> </n>
I added a notebook largest_component.ipynb which implements the largest component method for preprocessing. For each input image, a graph G = (V, E) is constructed. V is the set of nodes where the image intensites are above a certain threshold. E is an adjacency map between these nodes. Then the graph is divided into disjoint components (ie no edge joins any 2 components). The component which spans the largest area in the image is returned, and the input image is cropped with respect to that component. Then, all the images are rescaled to a fixed size of 30x30 pixels. If you try to run the code you'll see that the method works very well, however it is very slow. It takes about 75 seconds for 100 images, which means it would require about 2 hours for the entire dataset.
