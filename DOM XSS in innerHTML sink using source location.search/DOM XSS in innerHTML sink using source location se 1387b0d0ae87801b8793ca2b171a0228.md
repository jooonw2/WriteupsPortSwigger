# DOM XSS in innerHTML sink using source location.search

This lab contains a DOM-based cross-site scripting vulnerability in the search blog functionality. It uses an `innerHTML` assignment, which changes the HTML contents of a `div` element, using data from `location.search`.

To solve this lab, perform a cross-site scripting attack that calls the `alert` function.

Entramos a la maquina y tenemos un formulario

![image.png](image.png)

Ponemos `<img src=1 onerror=alert(1)>` o `<img src='0' onerror='alert()'>`

![image.png](image%201.png)

Nos salta la alerta

![image.png](image%202.png)