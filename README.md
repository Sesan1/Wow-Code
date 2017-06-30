# Wow-Code

public Node getReplacementNode(Node replacedNode){
		Node replacementParent = replacedNode;
		Node replacement = replacedNode;
		Node focusNode = replacedNode.rightChild;
		
		while (focusNode != null){
			replacementParent = replacement;
			replacement = focusNode;
			focusNode = focusNode.leftChild;
		}
		
		
		
		return replacement;
	}
