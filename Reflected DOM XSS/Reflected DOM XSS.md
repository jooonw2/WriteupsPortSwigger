# Reflected DOM XSS

This lab demonstrates a reflected DOM vulnerability. Reflected DOM 
vulnerabilities occur when the server-side application processes data 
from a request and echoes the data in the response. A script on the page
 then processes the reflected data in an unsafe way, ultimately writing 
it to a dangerous sink.

To solve this lab, create an injection that calls the `alert()` function.

Iniciamos la maquina y vemos que tenemos un formulario. Arrancamos el burpsuite y ponemos 

![image.png](image.png)

Tenemos la captura

![image.png](image%201.png)

Vemos el javascript

![image.png](image%202.png)

En la maquina ponemos lo siguiente en el formulario \"-alert(1)}//

![image.png](image%203.png)

Nos salta la alerta

![image.png](image%204.png)

![image.png](image%205.png)