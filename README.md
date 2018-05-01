# Make_up
import java.util.LinkedList;
import java.util.Scanner;
import java.util.Stack;

public class problem1 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner scan = new Scanner(System.in);
		while (scan.hasNext()) {
			Stack myStack1 = new Stack ();
			Stack myStack2 = new Stack ();
			Stack myStack0 = new Stack ();

			while (scan.hasNext()) {
				int n = scan.nextInt();
				switch (n) {
				case 2:
					myStack2.push(scan.nextLine());
				case 1:
					myStack1.push(scan.nextLine());
				case 0:
					myStack0.push(scan.nextLine());
				}
			}
			for (int i = 0; i < 10; i++) {
				if (myStack2.isEmpty())
					myStack2.push(0);
				if (myStack1.isEmpty())
					myStack1.push(0);
				if (myStack0.isEmpty())
					myStack0.push(0);
				System.out.println(myStack0.pop() + " " + myStack1.pop() + " " + myStack2.pop());
			}
		}
	}
}
