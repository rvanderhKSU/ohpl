<b>Introduction</b>

Developed by researchers at Kennesaw State University, OHPL directly addresses the unique requirements of the ordinal classification by using a point specific large margin loss function to group classes, while directly adhering to the ordinal information that are represented in the data. DNN’s built using OHPL perform on par with existing state-of-the-art ordinal classifiers on small datasets, while demonstrating vastly improved results on larger standard benchmark datasets.

<b>Usage</b>

There are currently two implementations of OHPL. OPHL Two-Stage, where you can train the model multiple times using ordering (centroid) loss function first, and then the point loss function. OPHLall, where you can incorporate ordering loss and point loss simultaneously. OPHLall offers two options: Mean Zero-One Error (MZE) and Mean Absolute Error (MAE). Mean loss is recommended in scenarios where you have, for example, 200 instances in a batch with 3 target classes. On the other hand, sum loss is recommended where you have, for example, 64 instances in a batch with 10 target classes.

<b>Citation</b>

If you use OHPL in a scientific publication, we would appreciate citations:

Vanderheyden, Bob, Ying Xie. Ordinal Hyperplane Loss. (2018). 2018 IEEE International Conference on Big Data (Big Data), Big Data (Big Data), 2018 IEEE International Conference On, 2337. https://doi-org.proxy.kennesaw.edu/10.1109/BigData.2018.8622079
