implementing DBSCAN
from sklearn.cluster import DBSCAN
import numpy as np

DBSCAN_cluster = DBSCAN(eps=2, min_samples=2).fit(data)
DBSCAN_cluster.labels_

plt.scatter(x, y, c=DBSCAN_cluster.labels_)
plt.show()
