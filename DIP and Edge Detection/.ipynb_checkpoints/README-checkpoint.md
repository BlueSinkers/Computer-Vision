# Edge Detection

This is one of those topics that is pretty implementation-heavy, and does require some amount of knowledge, but can easily be read and understood with minimal knowledge as well. Regardless, taking a look at my notes is a good idea. The structure of the folders:

- **images** - folder representing the input image (called 'lebronslam.jpg')
- **outputs** - folder representing all the outputs from each of the notebooks (so you can see the PNGs on their own); the naming convention is easy to understand, and make sure to check the notebooks if you want to understand what certain things mean

The actual Python Notebooks listed in order which you read (because certain documentation is omitted in the later notebooks becuase I discuss it in the initial ones)
- **gaussian_filter** - performs a simple Gaussian filter using OpenCV 
- **sobel_filter** - performs the Sobel filter using OpenCV and computes the partials (Sobel_X and Sobel_Y) and also the magnitude of the filter per the image - note that this is a gradient-based edge detection algorithm
- **laplacian_filter** - performs the Laplacian filter 
- **canny_filter** - runs the Canny Edge Detection Algorithm (NOT filter) on the input image, and outputs the image side by side with the initial image 
- **hough_transform** -- basically runs the Hough Transform for lines (which pretty neatly generalizes to the one for Circles or the Generalized Hough Transform as referred to in my notes) on the input image and outputs the image side by side with the intial image
- **SIFT_descriptors** -- this compute the SIFT descriptors and shows them on my input image -- although none of the technical parts of the "algorithm" to compute the SIFT features are used in the implementation, it shows what the features generally tend to look like

Since all the output images are stored as PNGs in the **outputs** folder, if you are interested in comparing the results, feel free to take a look there. Otherwise, most of this section is a lot of just understanding how convolution, filters, and edge-detection algorithms work!