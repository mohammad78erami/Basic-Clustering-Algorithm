#For KMeans Algorithm, it's best to find the ideal number of clusters(K) first
#getting the best K using elbow
from sklearn.cluster import KMeans

data = list(zip(x, y))
inertias = []

#checking the output inertia with 1-11 nubmer of clusters
for i in range(1,11):
    kmeans = KMeans(n_clusters=i)
    kmeans.fit(data)
    inertias.append(kmeans.inertia_)

#plotting the results
plt.plot(range(1,11), inertias, marker='o')
plt.title('Elbow method')
plt.xlabel('Number of clusters')
plt.ylabel('Inertia')
plt.show()

#the elbow of the plot is our desired number for K
#implementing KMeans with the proper number of clusters
kmeans = KMeans(n_clusters=3)
kmeans.fit(data)

#plotting the results
plt.scatter(x, y, c=kmeans.labels_)
plt.show()
