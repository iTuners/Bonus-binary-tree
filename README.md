# Bonus-binary-tree
加分二叉树

题目：https://www.luogu.com.cn/problem/P1040

代码思路：转化成dp问题，f[i][j]表示由i号节点到j号节点组成的subtree的最大分数，则可以写出递归函数f[i][j]=max(f[i][k-1]*f[k+1][j]+f[k][k]),其中发f[k][k]可以直接表示k号节点的值，每次递归的同时求出f[i][j]取最大值对应的根节点root[i][j],最终f[1][n]表示最大值，用tree()函数根据root数组得到前序遍历结果。
