# Practica Nro. 1 - C#  
En ejercicios resueltos  básicos de C# 

## 🛠️ Construido con :

* [C#](https://es.wikipedia.org/wiki/C_Sharp) 
* [Visual Studio 2019](https://visualstudio.microsoft.com/es/vs/) - Editor de código.
* [Typora](https://www.typora.io/) - Redacción archivo .md.

## ✒️ Autor

**Sebastián Echazú** 

* [Facebook](https://www.facebook.com/sebastian.echazu.1)
* [Instagram](https://www.instagram.com/seba_storm)
* [Twitter](https://twitter.com/seba_storm)
* [Github](https://github.com/SebastianEchazu)

------

## 1 - Saludos

En este ejercicio utilizará Visual Studio para escribir un programa C#. El programa le preguntará cómo se llama y luego le saludará por su nombre. 

### Para crear un programa C# nuevo

1. Inicie Microsoft Visual Studio .NET. 

2. En el menú File (Archivo), señale New (Nuevo) y pulse Project (Proyecto). 
3. Pulse Visual C# Projects en el cuadro Project Types (Tipos de proyecto). 
4. Pulse Console Application (Aplicación de consola) en el cuadro Templates (Plantillas). 
5. Escriba Saludos en el cuadro Name (Nombre). 
6. Escriba la ubicación deseada para el proyecto en el cuadro Location (Ubicación) y pulse OK. 
7. Escriba un comentario adecuado para el resumen. 
8. Cambie el nombre de la clase a Saludar. 
9. Guarde el proyecto seleccionando Save All (Guardar todo) en el menú File. 

### Cómo escribir instrucciones para preguntar y saludar al usuario 

1. Inserte la siguiente línea en el método Main después de los comentarios TODO: string miNombre; 

2. Escriba una instrucción que pregunte el nombre a los usuarios. 
3. Escriba otra instrucción que lea la respuesta del usuario desde el teclado y la asigne a la cadena miNombre. 
4. Añada una instrucción más que imprima “Hola, miNombre” en pantalla (donde miNombre es el nombre escrito por el usuario). 
5.  Una vez terminado, el método Main debe contener lo siguiente: 


```c#
static void Main(string[ ] args) {   
    string miNombre; 
    Console.WriteLine("Por favor, escriba su nombre");
    miNombre = Console.ReadLine( );  
    Console.WriteLine("Hola {0}", miNombre);
  } 
```

Guarde el trabajo realizado.  

### Cómo compilar y ejecutar el programa 

1. En el menú Build, seleccione Build Solution (o pulse CTRL+SHIFT+B). 
2. Corrija los posibles errores de compilación y vuelva a compilar si es necesario.
3. En el menú Debug, seleccione Start Without Debugging (o pulse CTRL+F5). 
4. En la ventana de consola que se abrirá, escriba su nombre cuando se lo pida el programa y pulse INTRO. 
5. Después de ver el saludo, pulse una tecla cuando aparezca el mensaje “Pulse cualquier tecla para continuar”. 



## 2 - Dividir

En este ejercicio escribirá un programa que utiliza tratamiento de excepciones para capturar errores inesperados en tiempo de ejecución. El programa pide al usuario dos valores enteros, divide el primero por el segundo y muestra el resultado. 

### Para crear un programa C# nuevo 

1. Inicie Visual Studio .NET si aún no se está ejecutando. 
2. En el menú File, señale New y pulse Project. 
3. Pulse Visual C# Projects en el cuadro Project Types. 
4. Pulse Console Application en el cuadro Templates. 
5. Escriba Divisor en el cuadro Name.
6. Escriba la ubicación deseada para el proyecto en el cuadro Location (Ubicación) y pulse OK. 
7. Escriba un comentario adecuado para el resumen. 
8. Cambie el nombre de la clase a Dividir. 
9. Guarde el proyecto seleccionando Save All en el menú File. 

### Cómo escribir instrucciones para pedir dos enteros al usuario 

1. En el método Main, escriba una instrucción que pida al usuario el primer entero. 
2. Escriba otra instrucción que lea la respuesta del usuario desde el teclado y la asigne a una variable llamada temp de tipo string. 
3. Añada la siguiente instrucción para convertir el valor de la cadena de temp en un entero y almacenar el resultado en i: int i = Int32.Parse(temp); 

4. Añada al código instrucciones para: 

   a. Pedir al usuario el segundo entero. 

   b. Leer la respuesta del usuario desde el teclado y asignarla a temp. 

   c. Convertir el valor de temp en un entero y almacenar el resultado en j. 

   El código debería ser parecido al siguiente: 

   ```c#
   Console.WriteLine("Escriba el primer entero");
   string temp = Console.ReadLine( ); 
   nt i = Int32.Parse(temp); 
   
   Console.WriteLine("Escriba el segundo entero"); 
   temp = Console.ReadLine( ); 
   int j = Int32.Parse(temp); 
   ```

5. Guarde el trabajo realizado. 

### Cómo dividir el primer entero por el segundo y mostrar el resultado 

1. Cree una nueva variable entera k que reciba el valor resultante de dividir i entre j, e insértelo al final del procedimiento anterior. 

   El código debería ser como esto: int k = i / j; 

2. Añada una instrucción para mostrar el valor de k. 3. Guarde el trabajo realizado. 

### Cómo probar el programa 

1. En el menú Debug, seleccione Start Without Debugging (o pulse CTRL+F5). 
2. Escriba 10 como valor del primer entero y pulse INTRO. 
3. Escriba 5 como valor del segundo entero y pulse INTRO. 
4. Compruebe que el valor de k que aparece es 2. 
5. Pulse CTRL+F5 para volver a ejecutar el programa. 
6. Escriba 10 como valor del primer entero y pulse INTRO. 
7. Escriba 0 como valor del segundo entero y pulse INTRO.
8. El programa provoca el lanzamiento de una excepción (división por cero). 
9. Pulse No para que desaparezca el cuadro de diálogo de la depuración Justin-Time. 

### Cómo añadir tratamiento de excepciones al programa 

1. Ponga el código del método Main dentro de un bloque try, como se indica a continuación: 

   ```c#
   try {Console.WriteLine (...); 
        ...    int k = i / j;  
        Console.WriteLine(...);
       } 
   ```

   

2. Añada a Main una instrucción catch después del bloque try. La instrucción catch tiene que imprimir un mensaje corto, como se ve en este código: 

   ```c#
   catch(Exception e) {   Console.WriteLine("Excepción lanzada: {0}" , e); } ... 
   ```

   

3. Guarde el trabajo realizado. 

------

## 🎁 Expresiones de Gratitud 

* Comenta a otros sobre este proyecto 📢
* Invita una cerveza 🍺 o un café ☕ al autor.  🤓. 

---

⌨️ con ❤️ por [Sebastian Echazu](https://github.com/SebastianEchazu) 😊
