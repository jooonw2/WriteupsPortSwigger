# Username enumeration via response timing

Fuerza bruta 

Atrapamos la solicitud y selecionamos lo que hemos rellenado en user y pass y lo añadimos. AÑDIMOS primero solo el usuario para comprobar cual es

![image.png](image.png)

Ahora en payloads le copiamos el diccionario y lanzamos el ataque

![image.png](image%201.png)

Podemos ver que todos nos devuelve codigo 200. Aunque no haya sido correcta la utenticación. Debemos fijarnos en Length, le damos clic al usuario y podemos ver la respuesta. En todos da incorrect user menos en este

![image.png](image%202.png)

Hacemos el mismo proceso poniendo user porque era el usuario que hemos encontrado y ahora probamos la contraseña y nos da la contraseña

![image.png](image%203.png)

Otro ataque diferente. Ahora vamos a añadir en Settings el error de Invalid user and password.

![image.png](image%204.png)

Vemos que hay uno que es diferente

![image.png](image%205.png)

Ahora buscamos la contraseña

![image.png](image%206.png)

**Username enumeration via response timing**

Nos da un usuario y una contraseña. Atrapamos el user y pass lo mandamos al Repeater

Copiamos esto

![image.png](image%207.png)

Lo copiamos aqui

![image.png](image%208.png)

Y en el request ponemos esto y vamos cambiando de uno en uno

![image.png](image%209.png)

Lo mandamos al intruder

![image.png](image%2010.png)

Ahora vamos a Payloads y en tipo ponemos numbers

![image.png](image%2011.png)

Y aqui ponemos pitchfork

![image.png](image%2012.png)

Volvemos a paylodas y ponemos en el 2

![image.png](image%2013.png)

Lanzamos el ataque y en los reslutados debemos ir a Columns y añadir response. Y vemos que hay un usuario que destaca

![image.png](image%2014.png)

Volvemos y limpiamos

![image.png](image%2015.png)

Y ponemos el diccionario de contraseña y lanzamos

![image.png](image%2016.png)