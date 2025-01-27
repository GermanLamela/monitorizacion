# Monitorización del Almacenamiento

## 1. Comando `free` (Memoria RAM)

El comando `free` muestra información sobre el uso de la memoria RAM (libre y utilizada).

### Opciones comunes:
- `-h`: Muestra los datos en un formato legible para humanos.
- `-t`: Incluye la memoria total en el resumen.
- `-s [segundos]`: Actualiza la información cada cierto intervalo de tiempo.

---

## 2. Comando `df` (Espacio en Disco)

El comando `df` permite conocer el uso y la disponibilidad del espacio en los sistemas de archivos (espacio de disco libre y utilizado).

### Opciones comunes:
- `-h`: Muestra los datos en un formato legible para humanos.
- `-T`: Muestra el tipo de sistema de archivos.
- `-x [tipo]`: Excluye sistemas de archivos del tipo especificado.

---

## 3. Comando `du` (Uso de Espacio en Directorios)

El comando `du` calcula el espacio que ocupan los directorios y archivos concretos.

### Uso básico:
```bash
du [ruta]

