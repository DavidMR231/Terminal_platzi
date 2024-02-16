## Cómo comprimir y descomprimir archivos en la terminal

**Introducción:**

En este archivo README encontrarás información sobre cómo comprimir y descomprimir archivos en la terminal usando los formatos `.tar`, `.tar.gz` y `.zip`.

**Comprimiendo archivos con formato .tar:**

El formato `.tar` es un tipo de compresión popular en sistemas UNIX. Se utiliza para almacenar información de forma lineal, ideal para backups.

**Sintaxis:**

```
tar [opciones] [nombreDelArchivoComprimido] [archivoAComprimir]
```

**Opciones:**

* **-c:** Comprimir.
* **-f:** Especificar el archivo a comprimir o descomprimir.
* **-v:** Mostrar información detallada del proceso.
* **-z:** Comprimir con gzip (formato `.tar.gz`).

**Ejemplos:**

* **Comprimir un archivo:**

```
tar -cf archivo.tar mi_archivo.txt
```

* **Comprimir un directorio:**

```
tar -cf archivo.tar directorio/
```

* **Ver el proceso de compresión:**

```
tar -cvf archivo.tar Documents/toCompress/
```

* **Comprimir con formato .tar.gz:**

```
tar -czvf archivo.tar.gz Documents/toCompress/
```

**Descomprimiendo archivos .tar:**

* **Descomprimir un archivo:**

```
tar -xf archivo.tar
```

* **Descomprimir un archivo .tar.gz:**

```
tar -xzvf archivo.tar.gz
```

**Comprimiendo archivos con formato .zip:**

El formato `.zip` es un formato de compresión universal compatible con la mayoría de sistemas operativos.

**Sintaxis:**

* **Comprimir:**

```
zip -r archivo.zip carpeta/
```

* **Descomprimir:**

```
unzip archivo.zip
```

**Opciones:**

* **-r:** Comprimir una carpeta de forma recursiva.

**Tabla de comandos:**

| Comando | Función | Opciones |
|---|---|---|
| **tar** | Comprimir/descomprimir .tar | -c, -x, -f, -v, -z |
| **zip** | Comprimir/descomprimir .zip | -r |


