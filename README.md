# GetSize-of-Linkedlist
public class BTsize {
    public static class Node{
        int data;
        Node next;
        Node(int data)
        {
            this.data=data;
        }
    }
        public int GetSize(Node root)
        {
            if(root==null)
            {
                return 0;
            }
            return GetSize(root.next)+1;
        }
    
    public static void main(String[] args)
    {
        BTsize obj=new BTsize();
        Node root=new Node(2);
        Node root1=new Node(4);
        Node root2=new Node(3);
        root.next=root1;
        root1.next=root2;
       // obj.GetSize(root);
        System.out.println(obj.GetSize(root));
    }
}
