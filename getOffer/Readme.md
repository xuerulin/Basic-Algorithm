|  题目   | 描述  | 思路 |
|  -------  | ----  | ----|
| 01.reverse-linked-list  | 反转链表|三个指针:pre,cur,next |
| 02.merge-two-sorted-array  | 合并两个排序的数组|选择一个有序数组进行拓展，给两个有序数组的尾部分别一个指针，比较尾部的大小，把大的插入到拓展数组的尾部|
|03.merge-two-sorted-lists|合并两个排序的链表|比较第一个元素，小的为主链表，另一个为次链表，主链表两个指针，次链表一个指针，遍历次链表，插入到主链表| 
|04.subtree-of-another-tree|判断B是不是A的子树|递归的方法，判断两个树匹配的必要条件是:A.val==B.val and match(A.left, B.left) and match(A.right, B.right)，判断B是不是A的子树的条件是：全匹配match(A,B) or match(A.left, B) or match(A.right,B)|
|05.mirror-binary-tree|镜像二叉树|1)就地镜像：root.left, root.right = root.right, root.left; mirror(root.left); mirrot(root.right)  2)创建节点镜像：newTree=TreeNode(root.val);newTree.left = mirror(root.right);newTree.right = mirror(root.left)|
|06.print-matrix|顺时针打印矩阵|每次打印当前矩阵的第一行，然后将剩余的矩阵逆时针旋转90度|
|07.level-print-binary-tree|按层打印二叉树|队列|
|08.afteroder-level-tree-bst|根据后序遍历数组判断是不是二叉搜索树|后序遍历根左右，二叉搜索树根左<根<根右|
|09.copy-random-linkedlist|拷贝复杂链表|1)原复杂链表主体复制 2)复制复杂链表的灵活指针 3)把复制的链表从原链表脱离|