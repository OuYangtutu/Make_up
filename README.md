# Make_up
import java.util.Scanner;
import java.util.Stack;

public class problem11 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner scan = new Scanner(System.in);
		// while(scan.hasNext()) {
		Stack myStack1 = new Stack();
		Stack myStack2 = new Stack();
		Stack myStack0 = new Stack();
		for (int i = 0; i < 30; i++) {
			if (scan.hasNext()) {
				int n = scan.nextInt();
				switch (n) {
				case 2:
					myStack2.push(scan.nextLine());
				case 1:
					myStack1.push(scan.nextLine());
				case 0:
					myStack0.push(scan.nextLine());
				}
			} else {
				if (myStack2.size() < 11)
					myStack2.push(0);
				if (myStack1.size() < 11)
					myStack1.push(0);
				if (myStack0.size() < 11)
					myStack0.push(0);
			}
		}
		for (int i = 0; i < 10; i++)
			System.out.println(myStack0.pop() + " " + myStack1.pop() + " " + myStack2.pop());
		// }
	}
}
