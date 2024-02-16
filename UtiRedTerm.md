## Utilidades de redes en la terminal

**Descripción:**

Este archivo describe algunas utilidades básicas de redes que se pueden usar en la terminal de Linux.

**Herramientas:**

* **ifconfig:** Muestra la configuración de las interfaces de red.

**Ejemplo:**

```
ifconfig
```

* **ip:** Muestra y manipula la configuración de las interfaces de red.

**Ejemplo:**

```
ip addr
```

* **ping:** Envía paquetes de prueba a un host para verificar la conectividad.

**Ejemplo:**

```
ping google.com
```

* **traceroute:** Muestra la ruta que toman los paquetes para llegar a un host.

**Ejemplo:**

```
traceroute google.com
```

* **nslookup:** Resuelve nombres de dominio a direcciones IP y viceversa.

**Ejemplo:**

```
nslookup google.com
```

* **dig:** Muestra información detallada sobre un nombre de dominio.

**Ejemplo:**

```
dig google.com
```

**Consejos:**

* Puedes usar el comando `man` seguido del nombre de la herramienta para obtener más información sobre cómo usarla.
* Puedes usar la tecla `Tab` para completar automáticamente los nombres de las herramientas y los argumentos.

**Ejemplos adicionales:**

* **Comprobar si hay una conexión a internet:**

```
ping 8.8.8.8
```

* **Encontrar la dirección IP de un host:**

```
ip addr show eth0 | grep inet
```

* **Verificar la configuración de DNS:**

```
cat /etc/resolv.conf
```

* **Cambiar la dirección IP de una interfaz de red:**

```
ip addr add 192.168.1.100/24 dev eth0
```

