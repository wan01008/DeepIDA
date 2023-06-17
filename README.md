# Deep IDA (Deep Integrative Discriminant Analysis) for Multi-view Data With Feature Ranking
A deep learning method for simultaneously integrating data from multiple sources and classifying subjects or units into one of two or more groups that permit variable ranking, and yields interpretable findings. The method also can be used in situations where variable ranking or selection is not needed.

1. Please check Reproducibility.ipynb for examples.

2. Datasets for the MNIST and simulation examples can be downloaded from: https://www.sandraesafo.com/software

3. Please cite this paper if you use this code for your research: https://arxiv.org/abs/2111.09964

Deep IDA: A Deep Learning Method for Integrative Discriminant Analysis of Multi-View Data with Feature Ranking by 
Jiuzhou Wang and  Sandra E. Safo.

These are the main functions found in main_functions.py. The helper_functions.py has functions called by the main functions. 

DeepIDA_nonBootstrap: For non-bootstrap option of Deep IDA. Does not implement variable ranking/selection. It returns the classification accuracy/labels based on DeepIDA+NCC (Deep IDA with nearest centroid classification), SVM on stacked or individual data, and the variables selected by Deep IDA+TS (Deep IDA + Teacher Student Network).

DeepIDA_VS: For implementing variable ranking/selection. It returns indices and figures (also in pdf) of top 10% selected variables in each view, and all feature importances in the csv files for users' interests.

DeepIDA_Bootstrap: Bootstrap version of Deep IDA. Calls the two functions above, and returns output from the two functions. 

4. Please send your comments and bugs to ssafo@umn.edu.
