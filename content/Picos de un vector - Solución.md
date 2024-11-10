```java
import java.util.Random;

public class peaks{
	public static void main(String[] args){
		Random rnd = new Random();
		int [] vec = new int [20];
		for (int i = 0; i < vec.length; i++){
			vec[i] = rnd.nextInt(100)+1;
		}
		for (int i = 0; i < vec.length; i++){
			System.out.print(vec[i] + " ");
		}
		
		System.out.println("\n\npicos:");
		if (vec[0] > vec[1])
			System.out.print(vec[0] + " ");
		for (int i = 1; i < vec.length-1; i++){
			if (vec[i] > vec[i-1] && vec[i] > vec[i+1])
				System.out.print(vec[i] + " ");
		}
		if (vec[vec.length-1] > vec[vec.length-2])
			System.out.print(vec[vec.length-1]);
	}
}
```