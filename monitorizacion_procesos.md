Monitorización de Procesos
==========================

En la administración de sistemas informáticos y redes, la monitorización de procesos es fundamental para garantizar el rendimiento, la estabilidad y la seguridad de los servidores. Linux proporciona herramientas en línea de comandos que permiten monitorizar el uso de CPU, memoria y otros recursos del sistema en tiempo real. Si algún comando no está instalado, puedes instalarlo con el siguiente comando:

`sudo apt install <nombre_comando>` 

1\. Comando ps
--------------

El comando ps proporciona una instantánea de los procesos en ejecución, mostrando información específica sobre ellos. Es útil para identificar procesos específicos o comprender cómo se distribuyen los recursos del sistema.

### Sintaxis básica:

`   ps [opciones]   `

### Opciones comunes:

*   **ps sin opciones**: Muestra los procesos asociados con la sesión actual del terminal.

*   ![Descripción de la imagen](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/ps.PNG)
    
*   **ps a**: Lista todos los procesos asociados a un terminal.

*  ![Descripción de la imagen](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/psa.PNG)
    
*   **ps aux**: Muestra todos los procesos en el sistema, incluyendo los que no están vinculados a un terminal.

*  ![Descripción de la imagen](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/psc.PNG)
    
*   **ps -C** : Filtra procesos por nombre. Ejemplo:
    

`   ps -C nano   `

* ![Descripción de la imagen](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/psc.PNG)

**Comentario**: Este comando es ideal para identificar procesos específicos o realizar un análisis rápido del sistema.

2\. Comando top
---------------

El comando top permite monitorizar el sistema en tiempo real, proporcionando una vista dinámica de los procesos en ejecución y el uso de recursos del sistema (CPU, memoria, etc.).

### Sintaxis básica:

`   top [opciones]   `

### Opciones comunes:

*   **top T**: Muestra el tiempo total de ejecución de los procesos.
    
*   **top M**: Ordena los procesos por uso de memoria.
    
*   **top P**: Ordena los procesos por uso de CPU.
    
*   **top p**: Muestra un proceso específico por su PID.
    
*   **top U** : Filtra los procesos de un usuario específico.
    
*   **top q**: Sale del comando sin confirmación.
    
*   **top k**: Permite finalizar un proceso ingresando su PID.
    

### Ejemplo:

`   top -u root   `
 ![Descripción de la imagen](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/top.PNG)

**Comentario**: Es una herramienta clave para detectar procesos que consumen demasiados recursos.

3\. Comando htop
----------------

htop es una versión mejorada de top, con una interfaz más interactiva y amigable. Ofrece funcionalidades adicionales como filtros, búsqueda y terminación de procesos.

### Sintaxis básica:

`   htop [opciones]   `

### Opciones:

*   **htop -u** : Filtra procesos de un usuario específico.

*   ![Descripción de la imagen](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/htopu.PNG)
    
*   **htop --tree**: Muestra los procesos en una vista jerárquica.

*    ![Descripción de la imagen](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/htoptree.PNG)
    
*   **htop -p** : Muestra información específica sobre uno o varios procesos por su PID.
    

### Atajos de Teclado:

*   **F2 (Setup)**: Configuración.
    
*   **F3 (Search)**: Búsqueda de procesos.
    
*   **F4 (Filter)**: Aplicar un filtro.
    
*   **F5 (Tree)**: Vista en árbol.
    
*   **F6 (Sort)**: Ordenar por diferentes parámetros.
    
*   **F9 (Kill)**: Terminar un proceso seleccionado.
    

**Comentario**: htop es ideal para usuarios que buscan una herramienta interactiva y visualmente intuitiva.

4\. Comando atop
----------------

atop es una herramienta avanzada que permite monitorizar procesos y otros recursos del sistema, como disco, red y memoria. Además, ofrece la capacidad de guardar registros para análisis posteriores.

### Uso básico:

*   atop

*   ![Descripción de la imagen](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/atop.PNG)
    
*   atop -r archivo\_de\_registro
    

**Comentario**: atop es una herramienta esencial para monitorear sistemas de forma detallada y con la posibilidad de analizar históricos.

5\. Comando vmstat
------------------

El comando vmstat proporciona información sobre el rendimiento del sistema, incluyendo procesos, memoria, paginación, bloques de E/S y uso de CPU.

### Sintaxis básica:

`   vmstat [intervalo] [repeticiones]   `

### Opciones comunes:

*   vmstat: Muestra un resumen general del estado del sistema.
    
*   vmstat 2 5: Muestra el estado del sistema cada 2 segundos durante 5 repeticiones.

*    ![Descripción de la imagen](https://github.com/GermanLamela/monitorizacion/blob/main/imagenes/vmstat.PNG)
    
*   vmstat -s: Proporciona estadísticas del sistema en formato de lista.
    

**Comentario**: Este comando es útil para analizar problemas de rendimiento y el uso general de los recursos del sistema.

Qué es el PID
-------------

El **PID** (_Process ID_ o Identificador de Proceso) es un número único asignado por el sistema operativo a cada proceso en ejecución. Este identificador permite a los administradores distinguir y gestionar procesos individuales. 


