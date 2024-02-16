## Guía de comandos básicos de la terminal de Linux

**Introducción:**

La terminal de Linux es una herramienta poderosa que te permite controlar tu sistema operativo y realizar una gran variedad de tareas. Aprender a usar algunos comandos básicos puede ayudarte a ser más eficiente y productivo.

**Comandos básicos:**

* **ls:** Lista los archivos y directorios en el directorio actual.

```
ls
```

* **cd:** Cambia el directorio actual.

```
cd directorio
```

* **mkdir:** Crea un nuevo directorio.

```
mkdir nombre_directorio
```

* **rm:** Elimina archivos y directorios.

```
rm archivo
```

* **cp:** Copia archivos y directorios.

```
cp archivo destino
```

* **mv:** Mueve o renombra archivos y directorios.

```
mv archivo nuevo_nombre
```

* **cat:** Muestra el contenido de un archivo en la pantalla.

```
cat archivo
```

* **grep:** Busca texto en archivos.

```
grep "texto" archivo
```

* **ps:** Muestra los procesos en ejecución.

```
ps
```

* **kill:** Detiene un proceso en ejecución.

```
kill pid
```

* **chmod:** Cambia los permisos de acceso a archivos y directorios.

```
chmod permisos archivo
```

* **sudo:** Permite al usuario realizar tareas con permisos de superusuario.

```
sudo comando
```

* **tar:** Crea y extrae archivos comprimidos.

```
tar -cvf archivo.tar.gz directorio
```

* **ssh:** Inicia una sesión segura de shell remota en otro sistema.

```
ssh usuario@host
```

* **ping:** Comprueba la conectividad de red.

```
ping host
```

* **python3:** Sirve para usar Python.

```
python3
```

* **exit():** Para salir de Python.

```
exit()
```

**Comandos adicionales:**

* **man:** Muestra la página de manual de un comando.

```
man comando
```

* **help:** Muestra ayuda para un comando específico.

```
comando --help
```

* **history:** Muestra el historial de comandos ejecutados.

```
history
```

* **clear:** Limpia la pantalla.
  
```
clear
```

## Cómo usar el comando `find`

**Descripción:**

El comando `find` es una herramienta poderosa para buscar archivos y directorios en sistemas Linux.

**Sintaxis básica:**

```
find [rutaDesdeDondeEmpezarBuscar] [opciones]
```

**Opciones:**

* **-type:** Especifica el tipo de archivo que se busca.
    * `f` para archivos
    * `d` para directorios
    * `l` para enlaces simbólicos
* **-name:** Especifica el nombre del archivo que se busca.
* **-mtime:** Especifica la fecha de modificación del archivo.
* **-ctime:** Especifica la fecha de creación del archivo.
* **-perm:** Especifica los permisos del archivo.

**Ejemplos:**

* **Buscar archivos que comienzan con la letra "f" en el directorio actual:**

```
find ./ -type f -name "f*"
```

* **Buscar archivos de 4 kilobytes en el directorio actual:**

```
find ./ -size 4k
```

* **Buscar archivos con permisos 755 en el directorio actual:**

```
find ./ -perm 755
```

## Cómo usar el comando `grep`

**Descripción:**

El comando `grep` es una herramienta para buscar líneas que coincidan con un patrón de texto en uno o más archivos.

**Sintaxis básica:**

```
grep [opciones] PATRON [ARCHIVO]
```

**Opciones:**

* **-i:** Ignora las mayúsculas y minúsculas.
* **-n:** Muestra el número de línea donde se encuentra la coincidencia.
* **-c:** Muestra el número de coincidencias en cada archivo.
* **-E:** Permite usar expresiones regulares.

**Ejemplos:**

* **Buscar todas las líneas que contienen la palabra "Hola" en el archivo "archivo.txt":**

```
grep Hola archivo.txt
```

* **Buscar todas las líneas que comienzan con la letra "A" en el archivo "archivo.txt", ignorando las mayúsculas y minúsculas:**

```
grep -i ^A archivo.txt
```

* **Mostrar el número de línea donde se encuentra la palabra "Hola" en el archivo "archivo.txt":**

```
grep -n Hola archivo.txt
```

* **Mostrar el número de coincidencias de la palabra "Hola" en el archivo "archivo.txt":**

```
grep -c Hola archivo.txt
```

* **Buscar todas las líneas que coincidan con la expresión regular "[0-9]{3}" (tres números) en el archivo "archivo.txt":**

```
grep -E "[0-9]{3}" archivo.txt
```

**Consejos:**

* Puedes usar el comando `man grep` para obtener más información sobre las opciones disponibles.
* Puedes usar el comando `grep -h` para mostrar el nombre del archivo antes de cada línea que coincida.
* Puedes usar el comando `grep -r` para buscar en un directorio de forma recursiva.

**Ejemplos adicionales:**

* **Buscar todas las líneas que contienen la palabra "Hola" en todos los archivos del directorio actual:**

```
grep -r Hola .
```

* **Mostrar el nombre del archivo y el número de línea donde se encuentra la palabra "Hola" en todos los archivos del directorio actual:**

```
grep -hn Hola .
```





