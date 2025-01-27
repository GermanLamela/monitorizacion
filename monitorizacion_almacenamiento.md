# Monitorización del Almacenamiento

## 1. Comando `free` (Memoria RAM)

El comando `free` muestra información sobre el uso de la memoria RAM (libre y utilizada).

### Opciones comunes:
- `-h`: Muestra los datos en un formato legible para humanos.
- ![Descripcion](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/freeh.PNG)
- `-t`: Incluye la memoria total en el resumen.
- ![Descripcion](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/freet.PNG)
- `-s [segundos]`: Actualiza la información cada cierto intervalo de tiempo.
- ![Descripcion](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/frees.PNG)

---

## 2. Comando `df` (Espacio en Disco)

El comando `df` permite conocer el uso y la disponibilidad del espacio en los sistemas de archivos (espacio de disco libre y utilizado).

### Opciones comunes:
- `-h`: Muestra los datos en un formato legible para humanos.
- ![-h](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/dfh.PNG)
- `-T`: Muestra el tipo de sistema de archivos.
- ![Descripcion](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/dft.PNG)
- `-x [tipo]`: Excluye sistemas de archivos del tipo especificado.
- ![Vaya coñazo](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/dfx.PNG)

---

## 3. Comando `du` (Uso de Espacio en Directorios)

El comando `du` calcula el espacio que ocupan los directorios y archivos concretos.

### Uso básico:

du [ruta]

- ![](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/du.PNG)

### Opciones comunes:

*   \-h: Muestra los datos en un formato legible para humanos.

*   ![](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/duh.PNG)
    
*   \-s: Muestra solo el total del espacio utilizado.

*   ![](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/dus.PNG)
    
*   \-d \[nivel\]: Especifica la profundidad del directorio que se desea analizar.

*   ![](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/dud.PNG)
    

4\. Comando iostat (Estadísticas de CPU y Disco)
------------------------------------------------

El comando iostat forma parte del paquete sysstat y ofrece información estadística sobre el uso del procesador y la actividad de los dispositivos de almacenamiento.

### Instalación:

`   sudo apt install sysstat   `

### Opciones comunes:

*   \-x: Muestra estadísticas detalladas de los dispositivos.

*   ![](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/iox.PNG)
    
*   \-d: Muestra estadísticas de entrada/salida de los discos.

*   ![](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/iod.PNG)
    
*   \-c: Muestra el uso del CPU.

*   ![](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/ioc.PNG)
    

5\. Comando ncdu (Visor Interactivo del Uso de Espacio)
-------------------------------------------------------

El comando ncdu es una herramienta interactiva para analizar el uso del espacio en los discos. Es ideal para identificar rápidamente directorios o archivos que ocupan mucho espacio.

### Instalación:

`   sudo apt install ncdu   `

### Uso básico:

`   ncdu [ruta]   `

- [](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/ncdu.PNG)

### Características principales:

*   Interfaz visual que permite navegar por los directorios y ver el espacio ocupado.
    
*   Posibilidad de eliminar archivos directamente desde la interfaz.
