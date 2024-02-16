## Manejo de archivos y procesos en la terminal

**Navegación por el sistema de archivos:**

* **`cd`**: Cambiar de directorio.
    * **Ejemplo:** `cd directorio/subdirectorio`
* **`ls`**: Listar el contenido de un directorio.
    * **Opciones:**
        * `-a`: Mostrar todos los archivos, incluyendo los ocultos.
        * `-l`: Mostrar información detallada de cada archivo.
        * `-h`: Mostrar tamaños de archivos en unidades legibles por humanos.
* **`pwd`**: Mostrar la ruta del directorio actual.

**Creación y eliminación de archivos y directorios:**

* **`mkdir`**: Crear un directorio.
    * **Ejemplo:** `mkdir nuevo_directorio`
* **`rmdir`**: Eliminar un directorio vacío.
    * **Ejemplo:** `rmdir directorio_vacio`
* **`touch`**: Crear un archivo vacío.
    * **Ejemplo:** `touch archivo.txt`
* **`rm`**: Eliminar un archivo.
    * **Opciones:**
        * `-f`: Eliminar sin preguntar.
        * `-r`: Eliminar directorios recursivamente.
        * `-i`: Preguntar antes de eliminar cada archivo.
    * **Ejemplo:** `rm archivo.txt`

**Copia y movimiento de archivos:**

* **`cp`**: Copiar archivos.
    * **Opciones:**
        * `-r`: Copiar directorios recursivamente.
        * `-f`: Forzar la copia, incluso si el archivo ya existe.
        * `-p`: Preservar los permisos y atributos del archivo original.
    * **Ejemplo:** `cp archivo.txt destino/archivo.txt`
* **`mv`**: Mover archivos.
    * **Opciones:**
        * `-r`: Mover directorios recursivamente.
        * `-f`: Forzar el movimiento, incluso si el archivo ya existe.
        * `-p`: Preservar los permisos y atributos del archivo original.
    * **Ejemplo:** `mv archivo.txt destino/archivo.txt`

**Manejo de procesos:**

**Ver los procesos activos (ps):**

El comando `ps` muestra los procesos que están activos en una tabla sencilla, donde la primera columna tiene el ID del proceso (PID) y la última el nombre.

**Opciones:**

* `-aux`: Mostrar información detallada de todos los procesos.
* `-u USUARIO`: Mostrar solo los procesos del usuario especificado.

**Ejemplo:**

```
ps aux
```

**Ver procesos más detallados (top):**

Si quieres ver una lista más detallada de los procesos con su consumo en CPU y RAM, además del usuario que lo activó, usa el comando `top`.

**Opciones:**

* `-u USUARIO`: Mostrar solo los procesos del usuario especificado.
* `-h`: Mostrar tamaños de memoria en unidades legibles por humanos.

**Ejemplo:**

```
top
```

**Filtrar por usuario:**

Presiona la tecla "u" para escribir el nombre del usuario por el cual quieres buscar.

**Salir:**

Presiona "q" para salir.

**Matar un proceso (kill):**

Para eliminar un proceso, usa el comando `kill` seguido del PID del proceso que quieres eliminar.

**Ejemplo:**

```
kill 595
```

**Nota:**

Este comando solo funciona para los procesos que se ejecutan en la terminal.

## Tabla de comandos

| Comando | Función | Opciones |
|---|---|---|
| **cd** | Cambiar de directorio | `directorio/subdirectorio` |
| **ls** | Listar el contenido de un directorio | `-a`, `-l`, `-h` |
| **pwd** | Mostrar la ruta del directorio actual | - |
| **mkdir** | Crear un directorio | `nuevo_directorio` |
| **rmdir** | Eliminar un directorio vacío | `directorio_vacio` |
| **touch** | Crear un archivo vacío | `archivo.txt` |
| **rm** | Eliminar un archivo | `-f`, `-r`, `-i` |
| **cp** | Copiar archivos | `-r`, `-f`, `-p` |
| **mv** | Mover archivos | `-r`, `-f`, `-p` |
| **ps** | Muestra una tabla con los procesos que se están ejecutando | `-aux`, `-u USUARIO` |
| **top** | Muestra una interfaz con los procesos que se están ejecutando, los recursos que consumen e información adicional | `-u USUARIO`, `-h` |
| **kill** | Mata el proceso que le indiques | PID |

