Обход в ширину

```
class Node:
    def __init__(self, value):
        self.value = value
        self.left = None
        self.right = None

class BinaryTree:
    def __init__(self):
        self.root = None

    def insert(self, value):
        if not self.root:
            self.root = Node(value)
            return

        current_node = self.root
        while True:
            if value < current_node.value:
                if not current_node.left:
                    current_node.left = Node(value)
                    break
                else:
                    current_node = current_node.left
            elif value > current_node.value:
                if not current_node.right:
                    current_node.right = Node(value)
                    break
                else:
                    current_node = current_node.right

    def breadth_first_traversal(self):
        if not self.root:
            return []

        queue = [self.root]
        result = []
        
        while queue:
            node = queue.pop(0)
            result.append(node.value)

            if node.left:
                queue.append(node.left)

            if node.right:
                queue.append(node.right)

        return result


# Example usage
tree = BinaryTree()
values = [24, 30, 36, 27, 20, 10, 5, 22, 40, 21]

for value in values:
    tree.insert(value)

print(tree.breadth_first_traversal()) # Output: [24, 20, 30, 10, 22, 27, 36, 5, 21, 40]
```

Daily quota: 9/10
ENG | ES | عربي | 中文 | فارسی
