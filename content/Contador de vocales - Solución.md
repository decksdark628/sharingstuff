```java
import java.util.Scanner;

public class vowelcounter{
	public static void main(String[] args){
		Scanner sc = new Scanner(System.in);
		int vowels = 0, a = 0, e = 0, i = 0, o = 0, u = 0;

		System.out.println("Escribe una palabra o frase");
		String word = sc.nextLine();

		for (int j = 0; j < word.length(); j++){
			if (word.charAt(j) == 'a' || word.charAt(i) == 'A'){
				vowels++;
				a++;
			}
			if (word.charAt(j)== 'e' || word.charAt(i) == 'E'){
				vowels++;
				e++;
			}
			if (word.charAt(j)== 'i' || word.charAt(i) == 'I'){
				vowels++;
				i++;
			}
			if (word.charAt(j)== 'o' || word.charAt(i) == 'O'){
				vowels++;
				o++;
			}
			if (word.charAt(j)== 'u' || word.charAt(i) == 'U'){
				vowels++;
				u++;
			}
		}
		System.out.println("vocales: " + vowels);
		System.out.println("A: " + a);
		System.out.println("E: " + e);
		System.out.println("I: " + i);
		System.out.println("O: " + o);
		System.out.println("U: " + u);
	}
}
```