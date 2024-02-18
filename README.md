# Clustering
## Comparitive performance study of different clustering algorithms using different pre-processing techniques with different numbers of clusters on different evaluation parameters
### Submitted by- CHELSI 3CS6 102117161    
Dataset used:  
Sales_Transactions_Dataset_Weekly Dataset consisting of 52 columns and 811 rows      
Algorithms used:  
1. K-means Clustering  
2. Hierarchial Clustering  
3. K-means shift Clustering
  
Pre-processing techniques used:  
1. No data preprocessing
2. Normalisation
3. Transformation
4. PCA
5. Normalisation & Transformation
6. Normalisation, Transformation & PCA  

For each algorithm, models are created using different pre-processing techniques and number of clusters- 3,4,5. The results are stored in form of a table & different graphs have been used for visualisation of the resuts from best models. Also, as seen in K-mean shift clustering the values obtained are 0 for all cases except with no data processing. This shows that this clustering algo isn't suitable for our dataset.  

Best Models:  
For K-means Clustering: Using no data processing with 3 no of clusters  
For Hierarchial Clustering: Using no data processing with 3 no of clusters  
For K-means shift Clustering: Using no data preprocessing with 3/4/5 no of clusters    

  Results:    
  For K-means Clustering:     
| Parameters        | No data preprocessing c=3 | No data preprocessing c=4 | No data preprocessing c=5 | Using Normalisation c=3 | Using Normalisation c=4 | Using Normalisation c=5 | Using Transform c=3 | Using Transform c=4 | Using Transform c=5 | Using PCA c=3 | Using PCA c=4 | Using PCA c=5 | Using N+T c=3 | Using N+T c=4 | Using N+T c=5 | Using N+T+PCA c=3 | Using N+T+PCA c=4 | Using N+T+PCA c=5 |
|-------------------|---------------------------|----------------------------|---------------------------|-------------------------|-------------------------|-------------------------|---------------------|---------------------|---------------------|---------------|---------------|---------------|---------------|---------------|---------------|-------------------|-------------------|-------------------|
| Silhouette        | 0.6141                    | 0.5666                     | 0.4538                    | 0.0259                  | 0.0152                  | 0.0126                  | 0.4764              | 0.4566              | 0.3645              | 0.4764        | 0.4566        | 0.3645        | 0.0231        | 0.0153        | 0.0077        | 0.0231            | 0.0152            | 0.0087            |
| Calinski-Harabasz | 3188.1254                 | 2601.2288                  | 2236.8582                 | 29.2165                 | 20.8758                 | 16.0717                 | 1877.8974           | 1845.174            | 1533.1167           | 1877.8974     | 1845.174      | 1533.1167     | 30.9255       | 22.0431       | 17.1368       | 30.9265           | 22.0381           | 17.1098           |
| Davies-Bouldin    | 0.6225                    | 0.8528                     | 0.9098                    | 5.7223                  | 7.8359                  | 9.1104                  | 0.8078              | 0.8721              | 1.2781              | 0.8078        | 0.8721        | 1.2781        | 6.0918        | 7.7155        | 9.2636        | 6.0829            | 7.6293            | 8.6375            |

For Hierarchial Clustering:    
| Parameters        | No data preprocessing c=3 | No data preprocessing c=4 | No data preprocessing c=5 | Using Normalisation c=3 | Using Normalisation c=4 | Using Normalisation c=5 | Using Transform c=3 | Using Transform c=4 | Using Transform c=5 | Using PCA c=3 | Using PCA c=4 | Using PCA c=5 | Using N+T c=3 | Using N+T c=4 | Using N+T c=5 | Using N+T+PCA c=3 | Using N+T+PCA c=4 | Using N+T+PCA c=5 |
|-------------------|---------------------------|----------------------------|---------------------------|-------------------------|-------------------------|-------------------------|---------------------|---------------------|---------------------|---------------|---------------|---------------|---------------|---------------|---------------|-------------------|-------------------|-------------------|
| Silhouette        | 0.6123                    | 0.5675                     | 0.4533                    | 0.0258                  | 0.0149                  | 0.0109                  | 0.4745              | 0.4605              | 0.363               | 0.4745        | 0.4605        | 0.363         | 0.0227        | 0.0155        | 0.0074        | 0.0227            | 0.0155            | 0.0074            |
| Calinski-Harabasz | 3091.1022                 | 2581.5766                  | 2232.213                  | 28.9372                 | 20.7535                 | 16.1339                 | 1864.9927           | 1822.7091           | 1507.7948           | 1864.9927     | 1822.7091     | 1507.7948     | 30.7747       | 21.9195       | 17.0919       | 30.7747           | 21.9195           | 17.0919           |
| Davies-Bouldin    | 0.6278                    | 0.8658                     | 0.914                     | 5.6755                  | 7.9009                  | 8.7452                  | 0.8096              | 0.8394              | 1.2777              | 0.8096        | 0.8394        | 1.2777        | 6.1811        | 7.6878        | 9.3205        | 6.1811            | 7.6878            | 9.3205            |

For K-means shift Clustering:
  | Parameters        | No data preprocessing c=3 | No data preprocessing c=4 | No data preprocessing c=5 | Using Normalisation c=3 | Using Normalisation c=4 | Using Normalisation c=5 | Using Transform c=3 | Using Transform c=4 | Using Transform c=5 | Using PCA c=3 | Using PCA c=4 | Using PCA c=5 | Using N+T c=3 | Using N+T c=4 | Using N+T c=5 | Using N+T+PCA c=3 | Using N+T+PCA c=4 | Using N+T+PCA c=5 |
|-------------------|---------------------------|----------------------------|---------------------------|-------------------------|-------------------------|-------------------------|---------------------|---------------------|---------------------|---------------|---------------|---------------|---------------|---------------|---------------|-------------------|-------------------|-------------------|
| Silhouette        | 0.4958                    | 0.4958                     | 0.4958                    | 0                       | 0                       | 0                       | 0.5378              | 0.5378              | 0.5378              | 0.5378        | 0.5378        | 0.5378        | 0             | 0             | 0             | 0                 | 0                 | 0                 |
| Calinski-Harabasz | 256.5403                  | 256.5403                   | 256.5403                  | 0                       | 0                       | 0                       | 1745.1555           | 1745.1555           | 1745.1555           | 1745.1555     | 1745.1555     | 1745.1555     | 0             | 0             | 0             | 0                 | 0                 | 0                 |
| Davies-Bouldin    | 1.0336                    | 1.0336                     | 1.0336                    | 0                       | 0                       | 0                       | 0.6386              | 0.6386              | 0.6386              | 0.6386        | 0.6386        | 0.6386        | 0             | 0             | 0             | 0                 | 0                 | 0                 |
