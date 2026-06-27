# Space Image Segmentation

For the Space Image Segmentation challenge we were given 2615 64x128 grayscale images of Mars terrain, with pixels categorized in 5 classes.

We built several versions of a U-net model, experimented with a Dual U-net too, and tried to improve the performance with image pre-processing layers.

We had to deal with:
- the low quality of the images
- the low quality of the masks
- the class imbalance among the pixels

Our best result on the test set was obtained with a 4 blocks and 2 stacks U-Net model, with an IoU of 0.62.

A better explanation of the work we did can be found [here](report_segmentation.pdf)

The code for the data analysis can be found [here](DataAnalysis_Final.ipynb)
The code for the U-Net model can be found [here](Unet _Final.ipynb) and the code for the Dual U-Net model can be found [here](DualUnet_Final.ipynb)
