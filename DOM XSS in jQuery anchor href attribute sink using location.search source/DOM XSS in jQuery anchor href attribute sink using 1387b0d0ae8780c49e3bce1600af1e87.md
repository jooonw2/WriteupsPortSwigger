# DOM XSS in jQuery anchor href attribute sink using location.search source

This lab contains a DOM-based cross-site scripting 
vulnerability in the submit feedback page. It uses the jQuery library's `$` selector function to find an anchor element, and changes its `href` attribute using data from `location.search`.

To solve this lab, make the "back" link alert `document.cookie`.

Iniciamos la maquina y vamos al apartado Submit feedback

![image.png](image.png)

En la URL añadimos lo siguiente

![image.png](image%201.png)

Vamos a inspeccionar elemento y buscamos lo que acabamos de añadir

![image.png](image%202.png)

volvemos a la URLy añadimos lo siguiente `javascript:alert(1)`

![image.png](image%203.png)

![image.png](image%204.png)