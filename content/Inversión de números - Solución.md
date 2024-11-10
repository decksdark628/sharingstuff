```java
import java.util.Scanner;

public class invertnums{
	public static void main(String[] args){
		Scanner sc = new Scanner(System.in);
		System.out.println("Escribe un numero");
		int num = sc.nextInt();

		System.out.println("numero invertido: ");
		for (int i = (num+"").length()-1; i >= 0; i--){
			System.out.print((num+"").charAt(i));
		}
	}
}
```