# Blind SQL injection with time delays

This lab contains a blind SQL injection vulnerability. The application uses a tracking cookie for analytics, and performs a SQL query containing the value of the submitted cookie.

The results of the SQL query are not returned, and the application does not respond any differently based on whether the query returns any rows or causes an error. However, since the query is executed synchronously, it is possible to trigger conditional time delays to infer information.

To solve the lab, exploit the SQL injection vulnerability to cause a 10 second delay.

Iniciamos la maquina , ponemos burpsuite a capturar y recargamos la pagina

![image.png](image.png)

En el campo TrackingId añadimos: `‘||pg_sleep(10)--` y lo enviamos

![image.png](image%201.png)

![image.png](image%202.png)