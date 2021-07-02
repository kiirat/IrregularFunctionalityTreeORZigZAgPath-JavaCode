# IrregularFunctionalityTreeORZigZAgPath-JavaCode
package yes;
import java.util.*;
public class zigzagORirregularFunctionalityTREE {

	//irregural tree formation

	public static void main(String[] args) {
		     	Scanner scn = new Scanner(System.in);
		     	int n = scn.nextInt();
		     	irregular(n);
		
		}
		public static void irregular(int n) {
			if(n==0) {
				return;
			}
			System.out.println(n+" ");   // pre  (left call)
			irregular(n-1);              // inline (mid call)
			System.out.println(n+" ");    // inline print 
			irregular(n-1);                  //right call (post)
			System.out.println(n+" ");     // post print
		}
}
