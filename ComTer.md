## Comandos de la terminal para comprimir archivos tar y zip

### Comprimir archivos con tar:

**Comprimir un archivo:**

```
tar -cf archivo.tar nombre_del_archivo
```

**Ejemplo:**

```
tar -cf archivo.tar mi_archivo.txt
```

**Comprimir un directorio:**

```
tar -cf archivo.tar directorio/
```

**Ejemplo:**

```
tar -cf archivo.tar mi_directorio/
```

**Comprimir y Gzip:**

```
tar -czf archivo.tar.gz nombre_del_archivo/directorio/
```

**Ejemplo:**

```
tar -czf archivo.tar.gz mi_archivo.txt
```

**Comprimir y Bzip2:**

```
tar -cjf archivo.tar.bz2 nombre_del_archivo/directorio/
```

**Ejemplo:**

```
tar -cjf archivo.tar.bz2 mi_directorio/
```

### Comprimir archivos con zip:

**Comprimir un archivo:**

```
zip archivo.zip nombre_del_archivo
```

**Ejemplo:**

```
zip archivo.zip mi_archivo.txt
```

**Comprimir un directorio:**

```
zip -r archivo.zip directorio/
```

**Ejemplo:**

```
zip -r archivo.zip mi_directorio/
```

**Comprimir con contraseña:**

```
zip -e archivo.zip nombre_del_archivo/directorio/ -P contraseña
```

**Ejemplo:**

```
zip -e archivo.zip mi_archivo.txt -P micontraseña
```

**Opciones adicionales:**

* `-v`: Muestra información detallada del proceso de compresión.
* `-t`: Muestra el contenido del archivo comprimido.
* `-x`: Descomprime un archivo comprimido.

**Ejemplo:**

```
tar -xvzf archivo.tar.gz
```
