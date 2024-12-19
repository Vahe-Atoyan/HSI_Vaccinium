# HSI_Vaccinium
This README provides a brief overview of the raw file processing pipeline, descriptions of the Data folder and subsequent steps involving Machine Learning and Dimensionality Reduction Visualization Techniques.

# Raw data processing
(Example pipeline is provided for the Gridzor Vu/Vm and Norway as  jupyter-notebook files RAW_HSI_Analysis_G_Vu-Vm.ipynb, RAW_HSI_Analysis_site.ipynb)

1. Download Data Files: Obtain the required .hdr and .raw files for the Dark Reference, White Reference, and Actual Data.
2. Calibrate the Hyperspectral Cube: Use the downloaded reference files (Dark and White) to calibrate the hyperspectral image.
3. Image Segmentation: Segment the hyperspectral image into two distinct classes—leaves and background—using K-means clustering.
Pixel Classification and Averaging:
4. Classify non-perimeter pixels of the segmented leaves in the hyperspectral image into their respective labels.
5. Compute the average spectrum for each leaf based on the classified pixels.
6. Save the resulting data as a .csv file for further analysis. (Data folder)


# Data folder description
G_Vu_Vm.csv - Vaccinium myrtillus and Vaccinium uliginosum from Gridzor

N-G-T-L_Sites_combined_zscore_data.csv - Vaccinium myrtillus only, from 4 different sites,  Norway (N), Gridzor (G), Tavush (T) and Lusagyugh (L) (z-score normalized data)

L    92
T    88
N    52
G    35



