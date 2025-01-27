# Monitorización de la Red

## 1. Comando `tcpdump`

`tcpdump` permite capturar y analizar el tráfico de red que pasa a través de una interfaz de red.

### Uso básico:
- `sudo tcpdump`: Captura todo el tráfico de red.
- `sudo tcpdump -i <nombre_interfaz>`: Captura el tráfico de una interfaz específica.
- `sudo tcpdump port <nº puerto>`: Filtra el tráfico por el número de puerto.

---

## 2. Comando `tcptrack`

`tcptrack` es una herramienta de monitorización en tiempo real que muestra conexiones TCP activas, direcciones IP origen y destino, puertos, estado de la conexión y cantidad de datos transmitidos en un formato visual.

### Uso básico:
```bash 
sudo tcptrack -i <nombre_interfaz>
```
3\. Comando iptraf-ng
---------------------

iptraf-ng es una herramienta interactiva que proporciona estadísticas detalladas sobre el tráfico de red en tiempo real.

### Uso básico:

1.  Entrar en el programa:
    

`   sudo iptraf-ng   `

1.  Seleccionar el tipo de monitorización.
    

4\. Comando netstat
-------------------

netstat es una herramienta clásica para inspeccionar conexiones de red, sockets y estadísticas.

### Instalación:

`   sudo apt-get install net-tools   `

### Uso básico:

*   netstat -a: Muestra todas las conexiones y puertos de escucha.
    
*   netstat -n: Muestra las direcciones y puertos en formato numérico.
    
*   netstat -tp: Muestra los procesos asociados a las conexiones.
    
*   netstat -l: Muestra solo los puertos que están en escucha.
    

5\. Comando ss
--------------

ss es una herramienta más moderna y eficiente que netstat para investigar conexiones de red. Proporciona información detallada sobre las conexiones TCP, UDP y otros protocolos.

### Uso básico:

*   ss -tuln: Muestra las conexiones TCP y UDP en escucha.
    
*   ss -s: Muestra estadísticas resumidas sobre las conexiones.
    
*   ss -p: Muestra los procesos que están utilizando las conexiones.
