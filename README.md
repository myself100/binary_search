# binary_search
package elclipse;
import java.util.*;
public class LinkedList {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		int a[]= {1,2,3,4,5,6,7,8,9,10};
		int n=a.length;
		int end=a.length-1;
		int search=14;
		binary(a,0,end,search); ///calling binary function
	
	
}
	public static void binary(int a[],int start,int end,int search) {
		  if(start>end) {
			  System.out.println("-1");
		}
		 int mid=(start+end)/2;   //calcutlating mid
		 if(a[mid]==search) {
			 System.out.print(mid+1);  //printing index.
		 }
		 else if(a[mid]<search) {
			 start=mid+1;
		 }
		 else if(a[mid]>search){
			 end=mid-1;
		 }
		 else {
			 System.out.println("not found"); /// if element not found
		 }
	}
	
}
