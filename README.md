# Unique_paths

给定一个矩阵，从左上角到右下角有几条不同的路。

思路：动态规划思想。到达每个点的情况有两种：从上面或从左边。即：P[i][j]=P[i][j-]+P[i-1][j]。
     注意初始化，将每个格子的数为1.
     vector<vector<int>> path(m,vector<int> (n,1))
