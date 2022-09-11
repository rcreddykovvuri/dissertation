This project is carried out on the tomato images dataset downloaded from https://data.mendeley.com/datasets/ngdgg79rzb/1.

The GitHub link for the entire coding is: https://github.com/rcreddykovvuri/dissertation.git


A brief view of the entire coding is explained below. 

Note:The vector generation is mostly placed along with the standard scaling code for all the dimensions.
==========================================================================================================================================================
Folder: 32     Description: Analysis of 32x32 dimension images.

files and description:
32_data.ipynb  - initial analysis of data conversion.

32_data_standard_scalar.ipynb  -  This file contains code for images to vector conversion of 32x32 data and analysis of standard scaled data.

32_data_minmax.ipynb and 32_data_minmax_v2.ipynb   -  These file contains analysis of minmax scaled data of 32x32 data.

32_data_no_scaling.ipynb, 32_data_no_scaling_v2.ipynb  -  These file contains analysis of data without scaling of 32x32 data. 

32_data_normalizer.ipynb, 32_data_normalizer_v2.ipynb   -  These files contains analysis of normalizer scaled data of 32x32 data. 
 

*****subfolder: PCA      Description: Analysis of PCA data of 32x32 data.
     Files and description:
     pca_32_32.ipynb   -  This file contains code to Scree plots of 32x32 data and generating vectors of PCA data. Saving them in the local system.

     pca_32_data_no_scaling, pca_32_data_standard_scaling_v2.ipynb  - This contains analysis on the PCA data of different vectors.

*****subfolder: no_bias  Description: Analysis of balanced images with 32x32 images.
     Files and description:
     32_data_standard_scalar.ipynb  -  This file contains code for images to vector conversion of 32x32 balanced data and analysis of standard scaled data.

     32_data_minmax.ipynb and 32_data_minmax_v2.ipynb   -  These file contains analysis of minmax scaled data of 32x32 balanced data.

     32_data_no_scaling.ipynb, 32_data_no_scaling_v2.ipynb  -  These file contains analysis of data without scaling of 32x32 balanced data. 

     32_data_normalizer.ipynb, 32_data_normalizer_v2.ipynb   -  These files contains analysis of normalizer scaled data of 32x32 balanced data. 
===========================================================================================================================================================
Folder: 64    Description:  Analysis of 64x64 dimension images.

files and description:
64_data_standard_scalar.ipynb  -  This file contains code for images to vector conversion of 64x64 data and analysis of standard scaled data with some algorithms.

64_data_standard_scaling_v2.ipynb  -  This file contains the analysis of standard scaled data of 64x64 data.

64_data_minmax.ipynb and 64_data_minmax_v2.ipynb   -  These file contains analysis of minmax scaled data of 64x64 data.

64_data_no_scaling.ipynb, 64_data_no_scaling_v2.ipynb  -  These file contains analysis of data without scaling of 64x64 data. 

64_data_normalizer.ipynb, 64_data_normalizer_v2.ipynb   -  These files contains analysis of normalizer scaled data of 64x64 data.

*****subfolder: PCA      Description: Analysis of PCA data of 64x64 data.
     Files and description:
     pca_64_64.ipynb   -  This file contains Scree plots of 64x64 data and generating vectors of PCA data.

     pca_64_data_no_scaling, pca_64_data_no_scaling_v2.ipynb  - This contains analysis on the PCA data of different vectors of 64x64 data.

*****subfolder: no_bias  Description: Analysis of balanced images with 64x64 images.
     Files and description:
     64_data_standard_scalar.ipynb  -  This file contains images to vector conversion of 64x64 balanced data and analysis of standard scaled data.

     64_no_bias_minmax.ipynb and 64_nobias_minmax_v2.ipynb   -  These file contains analysis of minmax scaled data of 64x64 balanced data.

     64_nobias_no_scaling.ipynb, 64_nobias_no_scaling_v2.ipynb  -  These file contains analysis of data without scaling of 64x64 balanced data. 

     64_nobias_normalizer.ipynb, 64_nobias_normalizer_v2.ipynb   -  These files contains analysis of normalizer scaled data of 64x64 balanced data.

============================================================================================================================================================
Folder: 64_other_features   Description: Analysis of 64x64 dimension images RGB vector along with mean, median, minimum, and maximum.

Files and description:
64_data_extraction.ipynb  - This file contains code to extract the new features and save the vectors.

64_data_no_scaling_v2.ipynb  -  This file contains code to fit the new features data with SVM (RBF).

============================================================================================================================================================
Folder: 128      Description: Analysis of 128x128 dimension images with RGB vector and standard scaling.

Files and Description:
128_data_standard_scalar.ipynb  - This file contains code for image to vector conversion and analysis on standard scaled data of 128x128 data.

128_data_standard_rbf.ipynb   -   This file contains code for fitting the data with SVM (RBF).

============================================================================================================================================================
Folder: CNN     Description: Analysis of 64x64 images with RGB, balanced(max count of 600 images for a disease), and Grayscale with CNN algorithm.

Files and Description:
grayscale_cnn.ipynb  -  Analysis of grayscale vector data of 64x64 data with CNN algorithm.

rgb_cnn.ipynb   -   Analysis of RGB vector of 64x64 data with CNN algorithm.

rgb_cnn_balanced.ipynb  -  Analysis of RGB vector of 64x64 data with balanced data with CNN algorithm.

rgb_cnn_more_epochs.ipynb  -  Analysis of RGB vector of 64x64 data with 10 epochs.

============================================================================================================================================================
Folder: validation  Description: validation of best models

Files and Description:
cross_validation_64_standard_scaling.ipynb  -  This contains the analysis of 64x64 data with standard scaling data with k-fold cross-validation.

statistical_test.ipynb   -   This contains the analysis of the statistical test between SVM (Poly) and SVM (RBF) of min-max data.

svm_roc.ipynb   -   This contains code for the AUC-ROC curve for the SVM (RBF) algorithm with 64x64 data of standard scaled data.

visualisation.ipynb  -  This contains code for visualizing class count.

============================================================================================================================================================
Folder: final_pickle_and_testing      Description:   creating pickle file, testing pickle file, and how to create back images from vectors.

Files and Description:
64_rbf_pickle_file.ipynb  -  Creating pickle file for SVM (RBF) model with 64x64 standard scaled data.

getting_images_from_vector.ipynb   -   creating images from the vector.

testing_pretrained_model.ipynb  -  code for testing the pretrained model.

============================================================================================================================================================
============================================================================================================================================================

How to test the model:

1. Download the dataset and Run the 64/64_data_standard_scalar.ipynb file for getting the vector data.
2. Run 64_rbf_pickle_file.ipynb program to save the svm.sav file in the local machine. Now you can use the model as many times you need.
3. Modify testing_pretrained_model.ipynb. In the first os.chdir give the downloaded path where svm.sav file is placed.
4. In the second os.chdir give the path where the input images are present.
5. Provide images names in input_images list.
6. run the entire code for testing the pickle file.


