# Reflected XSS into a JavaScript string with single quote and backslash escaped

This lab contains a reflected cross-site scripting 
vulnerability in the search query tracking functionality. The reflection
 occurs inside a JavaScript string with single quotes and backslashes 
escaped.

To solve this lab, perform a cross-site scripting attack that breaks out of the JavaScript string and calls the `alert` function.

Iniciamos la maquina y ponemos burpsuite a escuchar, rellenamos el formulario

![image.png](image.png)

Localizamos el paquete de búsqueda 

![image.png](image%201.png)

Añadimos lo siguiente en la primera línea para hacer la prueba. Y lo lanzamos.

![image.png](image%202.png)

Volvemos al formulario

![image.png](image%203.png)

Nos salta la alerta

![image.png](image%204.png)

![image.png](image%205.png)