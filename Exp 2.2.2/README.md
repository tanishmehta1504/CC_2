# CC-2-exp12 (24BDA70041)
## Problem Statement:285.Inorder Successor in BST
class Solution:

    def inorderSuccessor(self, root, p):
        successor = None
        while root:
            if p.val >= root.val:
                root = root.right
            else:
                successor = root
                root = root.left
        return successor