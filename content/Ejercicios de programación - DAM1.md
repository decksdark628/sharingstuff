Hola!👋 He creado unos ejercicios como manera de preparación para el examen.

Estan dividos en 3 categorias:
- **Simples** Nociones básicas
- **Intermedios** Para hacerte pensar, lo que imagino podría venir en el examen.
- **Extra** Como retos o curiosidades, probablemente no vengan en el examen

> [!tip] TIP: Puedes usar la tabla de contenidos a la izquierda para moverte rapidamente entre los distintos de niveles (En PC)

> [!warning]- ¿Errores al abrir los cuadros de explicación?
> Cierra y abre la pestaña que dice "click para ver la respuesta" y se soluciona.

> [!bug]- ¿Tienes comentarios?
> Si tienes alguna consulta o has encontrado algún error, escribeme por Whatsapp o envia un correo a denuncias@patrickdg.slmail.me (Para evitar "spoilers")

> [!attention]+ Sobre los ejercicios
> - Asumir siempre:
> 	- `public class untitled{ }`
> 	- `public static void main(String[] args){}`
> - Asumir solo si se utilizan:
> 	- `import java.util.Random;`
> 	- `import.java.util.Scanner;`
> - Cuando la respuesta es _no compila_:
> 	- Siempre será por solo una razón.
> 	- Esa razón nunca será:
> 		- Falta un corchete
> 		- Falta un punto y coma
> 		- Una palabra esta mal escrita
> 			- ejemplo: `pritnln` en vez de `println`

## Ejercicios simples
¿Sabes por qué no compilan?

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

---

## Ejercicios intermedios
¿Compila o no compila?

`if (compila == true)` ¿Qué sale?

`if (compila == false)` ¿Por qué?
### Ej. 0
```java
String saludo = "hola";

for (int i = 0; i < 4; i++){
	System.out.print(saludo.charAt(i));
} 
```

> [!example]- Click aquí para ver la respuesta
> **SI COMPILA**
>
> sale:
>
> ```
>hola
> ```
### Ej. 1
```java
String palabra = "DAM1";

if (palabra.charAt(4) == '1')
	System.out.println("si");
else
	System.out.println("no");
```

> [!example]- Click aquí para ver la respuesta
> **COMPILA, PERO DA ERROR**
>
> Razón: `charAt(4)` intenta acceder a una posición fuera del rango de la variable `palabra` (valores validos: 0, 1, 2, 3)

### Ej. 2
```java
Scanner sc = new Scanner(System.in);
int x = sc.nextInt();

if (x = 0)
	System.out.print("cero");
if (x > 0)
	System.out.print("positivo");
```

> [!example]- Click aquí para ver la respuesta
> **NO COMPILA**
>
> Razón: falta un `=` en el if

### Ej. 3
```java
String palabra = "DAM1";
boolean buleano = true;

System.out.println(palabra + buleano);
```

> [!example]- Click aquí para ver la respuesta
> **SI COMPILA**
>
> sale:
>
> ```
>DAM1true
> ```

### Ej. 4
```java
String nombre = "Jose Angel";

for (int i = 0; i < nombre.length; i++){
	System.out.print(nombre.charAt(i));
}
```

> [!example]- Click aquí para ver la respuesta
> **NO COMPILA**
>
> Razon: Para variables, el metodo es `.length()` con parentesis

### Ej. 5
```java
String [] vec = {"A"; "B"; "C"; "D"; "E"; "F"};

System.out.println(vec[1]);
System.out.println(vec[3]);
System.out.println(vec[5]);
```

> [!example]- Click aquí para ver la respuesta
> **NO COMPILA**
>
> Razon: usa `;` como separador de elementos del vector. Debería ser `,`

### Ej. 6
```java
char [] vec = {'D', 'A', 'M', '1'};

for (int i = 0; i < vec.length(); i++){
	System.out.print(vec[i]);
}
```

> [!example]- Click aquí para ver la respuesta
> **NO COMPILA**
>
> Razón: Para vectores, el metodo es  `.length` sin parentesis

### Ej. 7
```java
String [] vec = {"Lorem", "ipsum", "dolor", "sit", "amet"};

for (int i = 0; i <= 5; i+=2){
	System.out.print(vec[i] + " ");
}
```

> [!example]- Click aquí para ver la respuesta
> **SI COMPILA**
>
> sale:
>
> ```
> Lorem dolor amet
> ```
>
> > [!info]- Explicación
> >
> > `i` toma los valores `0, 2, 4` que corresponden a la primera, tercera y quinta palabra en el vector.
>

### Ej. 8
```java
char letra = 'a';

while (letra < 'e'){
	System.out.print(letra);
	letra++;
	System.out.print(letra);
	letra++;
	System.out.print(letra);
	letra++;
}
```

> [!example]- Click aquí para ver la respuesta
> **SI COMPILA**
>
> sale:
>
> ```
> abcdef
> ```

### Ej. 9
```java
boolean respuesta, respuestaValida = false;
int numero = 1;

while (!respuestaValida){
	switch (numero){
		case 0:
			System.out.println("NO");
			respuesta = false;
			respuestaValida = true;
		case 1:
			System.out.println("SI");
			respuesta = true;
			respuestaValida = true;
		default:
			System.out.println("ESCRIBE 1 O 2");
	}
}
```

> [!example]- Click aquí para ver la respuesta
> **SI COMPILA**
> 
> sale:
>
> ```
> SI
> ESCRIBE 1 O 2
> ```
>
>> [!info]- Explicación
>>
>> No hay breaks. Recorre todo el caso 1 y default antes de salir.
>

---

## Ejercicios extra
¿Compila o no compila?

- `if (compila == true)` ¿Qué sale?
- `if (compila == false)` ¿Por qué?

**Leyenda**
- 👁️: Agudeza visual, cosas que se te podrían pasar en un descuido
- ☝️🤓: Trivia, información rebuscada, curiosidades

### Ej. 0 ☝️🤓
```java
char a = '\n';

System.out.print(a);
```

> [!example]- Click aquí para ver la respuesta
> **SI COMPILA**
>
> sale:
>
> ```
> 
> ```
> 
> (Es decir, no sale nada ya que el caracter es un salto de linea)

### Ej. 1 👁️
```java
Scanner sc = new Scanner();

int numero;
char letra = 'e';

numero = sc.nextInt();
letra++;

System.out.println("letra: " + letra);
System.out.println("numero: " + numero);

```

> [!example]- Click aquí para ver la respuesta
> **NO COMPILA**
>
> Razón: Falta el `(System.in)` al crear un nuevo Scanner

### Ej. 2 ☝️🤓
```java
boolean verdadero = 1;
boolean falso = 0;

System.out.println(verdadero + " " + falso);
```

> [!example]- Click aquí para ver la respuesta
> **NO COMPILA**
>
> Razón: un boolean solo pueden ser ***true*** o ***false***

### Ej. 3 👁️
```java
Scanner sc = new Scanner(System.in);
int numero = sc.nextInt();

if (numero % 2 = 0)
	System.out.println("Es par");
else
	System.out.println("Es impar");
```

> [!example]- Click aquí para ver la respuesta
> **NO COMPILA**
>
> Razón: falta un `=` en el if

### Ej. 4 ☝️🤓
```java
int numero = 'A';
char letra = 10;
int temp = 0;

temp = numero;
numero = (int)letra;
letra = (char)temp;

System.out.println(letra);
System.out.println(numero);
```

> [!example]- Click aquí para ver la respuesta
> **SI COMPILA**
>
> sale:
>
> ```
> A
> 10
> ```

### Ej. 5 👁️
```java
char letras = 'A ';
int num = 10;

System.out.print(num + letras);
```

> [!example]- Click aquí para ver la respuesta
> **NO COMPILA**
>
> Razón: Hay un espacio luego de la 'A'. Variables de tipo char no pueden tener más de un carácter

### Ej. 6 👁️
```java
int [] vec = new int [10];

for (int i=0; i < vec.length; i++){
	Vec[i] = 5*i;
}
```

> [!example]- Click aquí para ver la respuesta
> **NO COMPILA**
>
> Razón: `Vec[i]` con mayuscula es distinto de `vec[i]`.

### Ej. 7 👁️
```java
int numero = 5, i = 0;
String texto = "10";

while (i =< 5){
	System.out.println(texto+numero);
	i++;
}
```

> [!example]- Click aquí para ver la respuesta
> **NO COMPILA**
>
> Razón: `=<` no es una comparación valida

### Ej. 8 👁️
```java
int [] vec = {0, 1, 1, 2, 3};

for (int i = 0, j = 1; i < vec.length-1; i++, j++){
	System.out.print(i + j);
	System.out.print(" ");
}
```

> [!example]- Click aquí para ver la respuesta
> **SI COMPILA**
>
> sale:
>
> ```
> 1 3 5 7
> ```
>
> > [!info]- Explicación
> >
> > `i` no es lo mismo que `vec[i]`
> >
> > `j` no es lo mismo que `vec[j]`
> > - 0+1 = 1
> > - 1+2 = 3
> > - 2+3 = 5
> > - 3+4 = 7
>

### Ej. 9 ☝️🤓
```java
char a = '\n';
char b = '"';
char c = ''';

System.out.print(a);
System.out.print(b);
System.out.print(c);
```

> [!example]- Click aquí para ver la respuesta
> **NO COMPILA**
>
> Razón: Las comillas simples se usan para señalar a java donde inicia y termina un char. 
>
> Para evitar conflictos debería ser escrito: `char c = '\'';`

---
`Fin del programa`