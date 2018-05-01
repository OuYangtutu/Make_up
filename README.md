# Make_up
import java.util.LinkedList;
import java.util.Scanner;

public class problem1 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner scan = new Scanner(System.in);
		while (scan.hasNext()) {
			LinkedList linkList2 = new LinkedList<Object>();
			LinkedList linkList1 = new LinkedList<Object>();
			LinkedList linkList0 = new LinkedList<Object>();

			while (scan.hasNext()) {
				int n = scan.nextInt();
				switch (n) {
				case 2:
					linkList2.push(scan.nextLine());
				case 1:
					linkList1.push(scan.nextLine());
				case 0:
					linkList0.push(scan.nextLine());
				}
			}
			for (int i = 0; i < 10; i++) {
				if (linkList2.isEmpty())
					linkList2.push(0);
				if (linkList1.isEmpty())
					linkList1.push(0);
				if (linkList0.isEmpty())
					linkList0.push(0);
				System.out.println(linkList0.pop() + " " + linkList1.pop() + " " + linkList2.pop());
				// if(linkList2.isEmpty()&&linkList1.isEmpty()&&linkList0.isEmpty())
				// System.out.println("0 "+"0 "+"0");
				// if(!linkList2.isEmpty()&&linkList1.isEmpty()&&linkList0.isEmpty())
				// System.out.println("0"+" 0 "+linkList2.pop());
			}
			linkList1.clear();linkList2.clear();linkList0.clear();
		}
	}
}
