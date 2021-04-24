In this section, we evaluate the performance of various advanced traffic speed prediction methods on the graphstructured data, and the prediction results in the next 15 minute, 30 minute, and 60 minute (T=3, 6, 12) are shown in the table below
****
![PERFORMANCE OF TRAFFIC SPEED PREDICTION ON METR-LA.](https://github.com/xueyan-dut/Deep-Learning-on-Traffic-Prediction/blob/main/Experiment/Results/prediction-results.jpg)
****
STGCN applied ChebNet graph convolution and 1D convolution to extract spatial dependencies and temporal correlations. ASTGCN leveraged two attention layers on the basis of
STGCN to capture the dynamic correlations of traffic network
in spatial dimension and temporal dimension, respectively.
DCRNN was a cutting edge deep learning model for prediction, which used diffusion graph convolutional networks
and RNN during training stage to learn the representations of
spatial dependencies and temporal relations. Graph WaveNet
combined graph convolution with dilated casual convolution
to capture spatial-temporal dependencies. STSGCN simultaneously extracted localized spatio-temporal correlation information based on the adjacency matrix of localized spatiotemporal graph. GMAN used purely attention structures in
spatial and temporal dimensions to model dynamic spatiotemporal correlations.
