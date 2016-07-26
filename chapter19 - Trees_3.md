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
    //todo
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
