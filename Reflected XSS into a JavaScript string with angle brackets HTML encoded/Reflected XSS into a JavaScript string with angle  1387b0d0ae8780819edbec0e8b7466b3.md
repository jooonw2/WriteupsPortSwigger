# Reflected XSS into a JavaScript string with angle brackets HTML encoded

This lab contains a reflected cross-site scripting vulnerability in the 
search query tracking functionality where angle brackets are encoded. 
The reflection occurs inside a JavaScript string. To solve this lab, 
perform a cross-site scripting attack that breaks out of the JavaScript 
string and calls the `alert` function.
        

Accedemos a la maquina, ponemos burpsuite a escuchar y metemos información en el formulario.

![image.png](image.png)

Mandamos el paquete al repeater

![image.png](image%201.png)

Y lo volvemos a enviar

![image.png](image%202.png)

Comprobamos la información que acabamos de enviar

![image.png](image%203.png)

Volvemos al formulario y ponemos lo siguiente

![image.png](image%204.png)

Vemos que nos salta la alerta

![image.png](image%205.png)

![image.png](image%206.png)