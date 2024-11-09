## ¿Por qué no compila?

> [!attention]+ NOTA
> - Asumir en todos los ejercicios:
> 	- `public class untitled{ }`
> 	- `public static void main(String[] args){}`
> - Asumir solo si se utilizan:
> 	- `import java.util.Random;`
> 	- `import.java.util.Scanner;`
> - Si la respuesta es _no compila_:
> 	- Siempre será por solo una razón.
> 	- Esa razón nunca será:
> 		- Falta un corchete
> 		- Falta un punto y coma
> 		- Una palabra esta mal escrita
> 			- ejemplo: `pritnln` en vez de `println`
### Ej. 0
```java
int x = "5";

System.out.print(x);
```

> [!example]- Click aquí para ver la respuesta
> Razón: el valor `"5"` es un String, no un int
### Ej. 1
```java
mensaje = "Hola mundo";

System.out.print(mensaje);
```

> [!example]- Click aquí para ver la respuesta
> Razón: La variable `mensaje` no ha sido declarada
### Ej. 2
```java
int x = 5, y = 7;

x = x+2;
z = y+x;
System.out.println(z);

```

> [!example]- Click aquí para ver la respuesta
> Razón: La variable `z` no ha sido declarada
### Ej. 3
```java
char letras = 'abc';

System.out.print(letras);
```

> [!example]- Click aquí para ver la respuesta
> Razón: char no puede tener más de un carácter
### Ej. 4
```java
String numero = "4";
int a = (int)numero;

System.out.println(a*2);
```

> [!example]- Click aquí para ver la respuesta
> Razón: un string no puede ser transformado a int usando un casting
### Ej. 5
```java
a = 3;
b = 9;

if (a > b)
	System.out.println("a es mayor");
else
	System.out.println("b no es mayor");
```

> [!example]- Click aquí para ver la respuesta
> Razón: Las variables `a` y `b` no han sido declaradas
### Ej. 6
```java
double x = 10.5;
int y = 4.5;

System.out.println(x+y);
```

> [!example]- Click aquí para ver la respuesta
> Razón: La variable `y` es un int y no puede contener el valor `4.5`
### Ej. 7
```java
Scanner sc = new Scanner(System.in);

int numero = sc.nextInt;

System.out.println("numero: " + numero);
```

> [!example]- Click aquí para ver la respuesta
> Razón: Falta el parentesis del metodo `nextInt()`
### Ej. 8
```java
Scanner sc = new Scanner(System.in);
int numero;

int numero = sc.nextInt();

System.out.println(numero);
```

> [!example]- Click aquí para ver la respuesta
> Razón: La variable `numero` ya esta definida
### Ej. 9
```java
boolean salir;
String palabra1;
String palabra2;

while(salir == false){
	palabra1 = "hola";
	palabra2 = "mundo";
	System.out.println(palabra1 + " " + palabra2);
	salir = true;
}
```

> [!example]- Click aquí para ver la respuesta
> Razón: La variable `salir` no ha sido inicializada