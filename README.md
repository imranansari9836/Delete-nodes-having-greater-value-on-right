class Solution
{
    Node compute(Node head)
    {
      if(head==null || head.next==null) return head;
        head.next=compute(head.next);
        if(head.next.data>head.data){

            return head.next;

        }else{

            return head;

        }

    }
