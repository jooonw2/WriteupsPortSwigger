# DOM XSS in document.write sink using source location.search inside a select element

This lab contains a DOM-based cross-site scripting 
vulnerability in the stock checker functionality. It uses the JavaScript
 `document.write` function, which writes data out to the page. The `document.write` function is called with data from `location.search` which you can control using the website URL. The data is enclosed within a select element.

To solve this lab, perform a cross-site scripting attack that breaks out of the select element and calls the `alert` function.

Iniciamos la maquina y nos metemos en un producto, le damos al botón check stock

![image.png](image.png)

Sobre el botón le damos clic inspeccionar elemento y buscamos storeid

![image.png](image%201.png)

Escribimos lo siguiente en la URL `productId=1&storeId=abc123` y lo enviamos

![image.png](image%202.png)

Vemos como el desplegable ha cambiado y sale por defecto el que hemos metido.

![image.png](image%203.png)

Si inspeccionamos podemos ver como ha cambiado el codigo.

![image.png](image%204.png)

Ahora en la URL añadimos esto `productId=1&storeId="></select><img%20src=1%20onerror=alert(1)>`

![image.png](image%205.png)

Nos salta la alerta

![image.png](image%206.png)

![image.png](image%207.png)