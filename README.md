# Image-Rectification

## Project Steps

1) Obtain image.
2) Segment the door and the window with the segmentation histogram.
3) Apply a kernel filter to the door and the window that obtain the lines horizontal and vertical of the objects.
4) Define the canny edge detector( but do not use it because we use a custom kernel filter)
5) Define a function that based on the edges we apply a hough transform, obtain the lines, and apply the cross product to calculate the intersection points and finally, return to these intersection points.
6) Obtain the centre of the intersections using a k-means algorithm.
7) Obtain all the combinations of the possible centres of the clusters
8) Finally, calculate the transformation_matrix with this line, map it to infinity, and use it to select the best image.
9) Separate the pixels with the histogram and count the pixels of the door and the window.
10) Obtain the ratio

## Getting Started

### Prerequisites 

Ensure you have the following dependencies installed:

- [Python](https://www.python.org/)
- [NumPy](https://numpy.org/)
- [Matplotlib](https://matplotlib.org/)
- [Math](https://docs.python.org/3/library/math.html)

You can install the required Python packages using pip:

pip install -r requirements.txt

### Usage

1. Clone this repository to your local machine:

git clone https://github.com/AriolaLeka/Image-Rectification.git

2. Navigate to the project directory:

cd Image-Rectification/Rectification.ipynd

## Acknowledgement

This project was done in collaboration with Shega Likaj and Francisco Amoros Cubells.

