# DOM XSS in jQuery selector sink using a hashchange event

This lab contains a DOM-based cross-site scripting vulnerability on the home page. It uses jQuery's `$()` selector function to auto-scroll to a given post, whose title is passed via the `location.hash` property.

To solve the lab, deliver an exploit to the victim that calls the `print()` function in their browser.

Entramos a la maquina y vamos a go to exploit server

![image.png](image.png)

Copiamos toda la URL de la maquina `<iframe src="URL" onload="this.src +='<img src=x onerror=print()>' ">` y le damos a View exploit

![image.png](image%201.png)

Se nos abrirá lo siguiente, cancelamos.

![image.png](image%202.png)

Volvemos a atrás y le damos a Deliver exploit to victim

![image.png](image%203.png)

![image.png](image%204.png)