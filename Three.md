tree = BinaryTree()
for value in [24, 30, 36, 27, 20, 10, 5, 22, 40, 21]:
    tree.insert(value)

print(tree.breadth_first_traversal()) # [24, 20, 30, 10, 22, 36, 5, 21, 27, 40]
