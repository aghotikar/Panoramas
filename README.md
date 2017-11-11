# Panoramas

The goal of this project is to create Panoramas using:
 1. Homographies and perspective warping on a common plane (3 input images)
 2. Cylindrical warping (many images)

The code flow is as follows:
 1. Read in the images: input1.jpg, input2.jpg, input3.jpg
 2. [Apply cylindrical wrapping if needed]
 3. Calculate the transformation (homography for projective; affine for cylindrical) between each
 4. Transform input2 and input3 to the plane of input1, and produce output.png
 5. Perform Laplacian Blending to stitch the images together nicely
