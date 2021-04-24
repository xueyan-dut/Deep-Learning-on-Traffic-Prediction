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
<br><br><br>
As can be seen from the experimental results,
First, the attention-based methods (GMAN) perform better
than other GCN-based methods in extracting spatial correlations. When modeling spatial correlations, GCN uses sum,
mean or max functions to aggregate the features of each
node’s neighbors, ignoring the relative importance of different neighbors. On the contrary, the attention mechanism
introduces the idea of weighting to realize adaptive updating
of nodes at different times according to the importance of
neighbor information, leading to better results. Second, the
performance of the spectral models (STGCN and ASTGCN)
is generally lower than that of the spatial models (DCRNN,
Graph WaveNet and STSGCN). In addition, the results of
most methods are not significantly different for 15min, but
with the increase of the predicted time length, the performance
of the attention-based method (GMAN) is significantly better
than other GCN-based methods. Since most existing methods
predict traffic conditions in an iterative manner, and their
performance may not be greatly affected in short-term predictions because all historical observations used for prediction are
error-free. However, as long-term prediction has to produce the
results conditioned on previous predictions, resulting in error
accumulations and reducing the accuracy of prediction greatly.
Since the attention mechanism can directly perform multistep predictions, ground-truth historical observations can be
used regardless of short-term or long-term predictions, without
the need to use error-prone values. Therefore, the above
observations suggest possible ways to improve the prediction
accuracy. First, the attention mechanism can extract the spatial
information of road network more effectively. Second, the spatial-based approaches are generally more efficient than the
spectral-based approaches when working with GCN. Third,
the attention mechanism is more effective to improving the
performance of long-term prediction when modeling temporal
correlation. It is worth mentioning that adding an external data component is also beneficial for performance when external
data is available.
<br><br><br>
To evaluate the computation complexity, we compare the
computation time and the number of parameters among these
models on the METR-LA dataset. All the experiments are
conducted on the Tesla K80 with 12GB memory, the batchsize
of each method is uniformly set to 64, T is set to 12, and we
report the average training time of one epoch. For inference,
we compute the time cost on the validation data. The results
are shown in the table below.
****
![PERFORMANCE OF TRAFFIC SPEED PREDICTION ON METR-LA.](https://github.com/xueyan-dut/Deep-Learning-on-Traffic-Prediction/blob/main/Experiment/Results/prediction-results.jpg)
****
STGCN adopts fully convolutional
structures so that it is the fastest in training, and DRCNN
uses the recurrent structures, which are very time consuming.
Compared to methods (e.g., STGCN, DCRNN, ASTGCN,
STSGCN) that require iterative calculations to generate 12
predicted results, Graph WaveNet can predict 12 steps ahead
of time in one run, thus requiring less time for inference.
STSGCN integrates three graphs at different moments into
one graph as the adjacency matrix, which greatly increases
the number of model parameters. Since GMAN is a pure
attention mechanism model that consists of multiple attention
mechanisms, it is necessary to calculate the relation between
pairs of multiple variables, so the number of parameters is
also high. Note that, when calculating the computation time
of GMAN, it displays “out of memory” on our device, due to
the relatively complex design of the model.
