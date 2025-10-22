# Capítulo 2 - Manual práctico de Linux

## Ejercicios iniciales

**Muestra el contenido del directorio actual y luego el contenido del directorio que está justo a un nivel superior**

```powershell
ls
ls ..
```

![image.png](image.png)

**¿En qué día de la semana naciste?, utiliza la instrucción cal para averiguarlo.**

```powershell
cal -d 2002-02-08
```

![image.png](image%201.png)

**Muestra los archivos del directorio `/bin`**

```powershell
ls /bin
```

![image.png](image%202.png)

**Suponiendo que te encuentras en tu directorio personal (`/home/nombre`), muestra un listado del contenido de `/usr/bin`**

- **Con una sola línea de comando**

```powershell
ls /usr/bin
```

![image.png](image%203.png)

- **Moviéndote paso a paso por los directorios**

```powershell
cd ..
cd ..
cd usr
cd bin
ls
```

![image.png](image%204.png)

- **Con dos líneas de comandos.**

```powershell
cd /usr/bin
ls
```

![image.png](image%205.png)

**Muestra todos los archivos que hay en `/etc` y todos los que hay dentro de cada subdirectorio, de forma recursiva (con un solo comando).**

```powershell
ls /etc/*/
```

![image.png](image%206.png)

**Muestra todos los archivos del directorio /etc ordenados por tamaño (de mayor a menor) junto con el resto de características, es decir, permisos, tamaño, fechas de la última modificación, etc. El tamaño de cada fichero debe aparecer en un formato “legible”, o sea, expresado en Kb, Mb, etc.**

```powershell
ls  -l -h -S -s /etc
```

![image-20250926105913660.png](image-20250926105913660.png)

**Muestra todos los archivos del directorio `/bin` ordenados por tamaño (de menor a mayor). Sólo debe aparecer el tamaño y el nombre de cada fichero, sin ninguna otra información adicional. El tamaño de cada fichero debe aparecer en un formato “legible”, o sea, expresado en Kb, Mb, etc.**

```powershell
ls -h -Sr -s /bin
```

![image-20250926111050249.png](image-20250926111050249.png)

**Muestra el contenido del directorio raíz utilizando como argumento de `ls` una ruta absoluta.**

```powershell
ls /
```

![image-20250926111225433.png](image-20250926111225433.png)

**Muestra el contenido del directorio raíz utilizando como argumento de `ls` una ruta relativa. Suponemos que el directorio actual es `/home/elena/documentos`.**

```powershell
ls ../../../
```

![image-20250926111623668.png](image-20250926111623668.png)

**Crea el directorio `gastos` dentro del directorio personal.**

```powershell
mkdir gastos
```

![image-20250926111813516.png](image-20250926111813516.png)