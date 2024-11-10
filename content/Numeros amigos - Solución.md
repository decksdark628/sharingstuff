```java
import java.util.Scanner;

public class numerosamigos{
	public static void main(String[] args){
		Scanner sc = new Scanner(System.in);
		int num1, num2, temp;
		boolean check1 = false, check2 = false;

		System.out.println("Escribe el primer numero");
		num1 = sc.nextInt();
		System.out.println("Escribe el segundo numero");
		num2 = sc.nextInt();

		temp = 1;
		for(int i = 2; i < num1; i++){
			if(num1 % i == 0)
				temp += i;
		}
		if (temp == num2)
			check1 = true;
		if (check1){
			temp = 1;
			for (int i = 2; i < num2; i++){
				if (num2 % i == 0)
					temp += i;
			}
			if (temp == num1)
				check2 = true;
		}
		if (check1&&check2)
			System.out.println("Si son amigos");
		else
			System.out.println("No son amigos");
	}
}
```