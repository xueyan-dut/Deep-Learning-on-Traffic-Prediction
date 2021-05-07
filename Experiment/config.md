In the experiment, we compare the performance of six typical speed prediction methods with public codes on a public dataset. The table below summarizes the links of public source codes for related comparison methods.<br>
|#|Approach|Link|
|---|----|-----|
|1|`STGCN`|https://github.com/VeritasYin/STGCN_IJCAI-18|
|2|`DCRNN`|https://github.com/liyaguang/DCRNN|
|3|`ASTGCN`|https://github.com/guoshnBJTU/ASTGCN-r-pytorch|
|4|`Graph WaveNet`|https://github.com/nnzhan/Graph-WaveNet|
|5|`STSGCN`|https://github.com/Davidham3/STSGCN| <br>

METR-LA dataset: This dataset contains 207 sensors and collects 4 months of data ranging from Mar 1st 2012 to Jun 30th 2012 for the experiment. 70% of data is used for training, 20% is used for testing while the remaining 10% for validation. Traffic speed readings are aggregated into 5 minutes windows, and Z-Score is applied for normalization. To construct the road network graph, each traffic sensor is considered as a node, and the adjacency matrix of the nodes is constructed by road network distance with a thresholded Gaussian kernel
We use the following three metrics to evaluate different models: Mean Absolute Error (MAE), Rooted Mean Squared Error (RMSE), and Mean Absolute Percent Error (MAPE).<br>
<img src="https://latex.codecogs.com/png.image?\dpi{110}&space;MAE=\frac{1}{\xi&space;}\sum_{i=1}^{\xi&space;}\left|&space;\hat{y}^{i}-y^{i}\right|" title="MAE=\frac{1}{\xi }\sum_{i=1}^{\xi }\left| \hat{y}^{i}-y^{i}\right|" />
&#8194;&#8194;&#8194;&#8194;&#8194;&#8194;&#8194;&#8194;&#8194;
<img src="https://latex.codecogs.com/png.image?\dpi{110}&space;RMSE&space;=&space;\sqrt{\frac{1}{\xi&space;}\sum_{i=1}^{\xi&space;}\left&space;(&space;\hat{y}^{i}-y^{i}&space;\right&space;)^{2}}" title="RMSE = \sqrt{\frac{1}{\xi }\sum_{i=1}^{\xi }\left ( \hat{y}^{i}-y^{i} \right )^{2}}" />
&#8194;&#8194;&#8194;&#8194;&#8194;&#8194;&#8194;&#8194;&#8194;
<img src="https://latex.codecogs.com/png.image?\dpi{110}&space;MAPE&space;=&space;\frac{1}{\xi&space;}\sum_{i=1}^{\xi&space;}\left|&space;\frac{\hat{y}^{i}-y^{i}&space;}{y^{i}}\right|*100%" title="MAPE = \frac{1}{\xi }\sum_{i=1}^{\xi }\left| \frac{\hat{y}^{i}-y^{i} }{y^{i}}\right|*100%" /><br>
where <img src="https://latex.codecogs.com/png.image?\dpi{110}&space;\hat{y}^{i}" title="\hat{y}^{i}" /> and <img src="https://latex.codecogs.com/png.image?\dpi{110}&space;{y}^{i}" title="{y}^{i}" /> denote the predicted value and the ground truth of region i for predicted time step, and ξ is the total number of samples.
