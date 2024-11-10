```java
import java.util.Scanner;

public class raizdigital{
	public static void main(String[] args){
		Scanner sc = new Scanner(System.in);
		int num, sum = 0;
		boolean oneDigit = false;

		System.out.println("Escribe un numero");
		num = sc.nextInt();

		while(!oneDigit){
			sum = 0;
			for (int i = 0; i < (num+"").length(); i++){
				sum += Integer.parseInt((num+"").charAt(i)+"");
			}

			if (sum/10 == 0)
				oneDigit = true;
			else
				num = sum;
		}
		System.out.println("La raiz digital del numero es: " + sum);
	}
}
```