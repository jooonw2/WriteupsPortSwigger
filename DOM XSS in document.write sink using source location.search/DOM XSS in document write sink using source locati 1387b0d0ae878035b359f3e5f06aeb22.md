# DOM XSS in document.write sink using source location.search

This lab contains a DOM-based cross-site scripting 
vulnerability in the search query tracking functionality. It uses the 
JavaScript `document.write` function, which writes data out to the page. The `document.write` function is called with data from `location.search`, which you can control using the website URL.

To solve this lab, perform a cross-site scripting attack that calls the `alert` function.

Accedemos al laboratorio y vemos que tenemos un formulario

![image.png](image.png)

Primero hacemos una prueba, metemos información

![image.png](image%201.png)

Vamos a inspeccionar elemento y buscamos lo que acabamos de insertar. Vemos que lo ha intentado cargar como una imagen

![image.png](image%202.png)

Volvemos al formulario y ponemos lo siguiente

![image.png](image%203.png)

Y nos salta la alerta

![image.png](image%204.png)