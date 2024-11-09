# Blind SQL injection with conditional errors

Entraremos en la maquina ponemos burp a interceptar el trafico y recargamos la pagina. Una vez interceptada la pagina la mandamos al repeater.

![image.png](image.png)

Hacemos la siguiente prueba. Con una Comilla.

![image.png](image%201.png)

Ahora hacemos la prueba con dos comillas y vemos que temenos diferentes respuestas. Tenemos un SQLi

![image.png](image%202.png)

Verificamos que en la table users de la base de datos hay un registro llamado administrator

![image.png](image%203.png)

Añadimos el 1 para ver como es de larga la contraseña

![image.png](image%204.png)

Añadimos del 1 al 25 para revisar los caracteres que tiene.

![image.png](image%205.png)

Una vez lanzado vemos que que cambia a partir de 21. Eso signfica que la contraseña tiene 20 caracteres.

![image.png](image%206.png)

Entonces ahora temenos que descubrir uno a uno los caracteres de la contraseña.

![image.png](image%207.png)

En paylodas deberemos meter todas las letras y numeros.

![image.png](image%208.png)

Sacamos el primer caracter.

![image.png](image%209.png)

Ahora deberemos sacar los demas caracteres. Deberemos ir cambiando el numero (hasta 20) para conseguir todos los caracteres.

![image.png](image%2010.png)

Una vez tenemos los 20 digitios ya habriamos conseguido la contraseña

![image.png](image%2011.png)