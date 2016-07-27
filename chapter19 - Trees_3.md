## Chapter 19 - Trees, Part III
__Page 166__

### AVL Trees

__C#__
```c#
class AVLNode {
  public int val;
  public int balance;
  public AVLNode right;
  public AVLNode left;

  public AVLNode(int value){
    val = value;
    balance = 0;
    right = null;
    left = null;
  }

  public int Height() {
    int leftHeight = 0;
    int rightHeight = 0;
    if(!left && !right){
      return 1;
    }
    if(left){
      leftHeight = left.Height();
    }
    if(right){
      rightHeight = right.Height();
    }
    return 1 + (leftHeight > rightHeight ? leftHeight : rightHeight);
  }

  public bool IsBalanced(){
    bool leftBalanced = true;
    bool rightBalanced = true;

    if(left){
      leftBalanced = left.IsBalanced();
    }
    if(right){
      rightBalanced = right.IsBalanced();
    }
    if(Math.Abs(balance) > 1){
      return false;
    }
    return (leftBalanced && rightBalanced);
  }
}

class AVLTree {
  public AVLNode root;

  public AVLTree(){
    root = null;
  }

  public null Add(value){
    if(!root){
      root = new AVLNode(value);
    } else {
      AVLNode current = root;
      while(current){
        if(value < current.val){
          //Update the Balance value of the current node
          current.balance--;
          //go left if a node exists there, otherwise place the new node
          if(current.left){
            current = current.left;
          } else {
            current.left = new AVLNode(value);
            return;
          }
        } else {
          //Update the Balance value of the current node
          current.balance++;
          //go right if a node exists there, otherwise place the new node
          if(current.right){
            current = current.right;
          } else {
            current.right = new AVLNode(value);
            return;
          }
        }
      }
    }
  }

  public AVLNode Remove(value){
    //todo
  }

  public int Height(){
    if(root){
      return root.Height();
    }
    return 0;
  }

  public bool IsBalanced(){
    if(root){
      return root.IsBalanced();
    }
    return true;
  }
}
```
