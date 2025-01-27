onitorización de Procesos
==========================

En la administración de sistemas informáticos y redes, la monitorización de procesos es fundamental para garantizar el rendimiento, la estabilidad y la seguridad de los servidores. Linux proporciona herramientas en línea de comandos que permiten monitorizar el uso de CPU, memoria y otros recursos del sistema en tiempo real. Si algún comando no está instalado, puedes instalarlo con el siguiente comando:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`sudo apt install` 

1\. Comando ps
--------------

El comando ps proporciona una instantánea de los procesos en ejecución, mostrando información específica sobre ellos. Es útil para identificar procesos específicos o comprender cómo se distribuyen los recursos del sistema.

### Sintaxis básica:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   ps [opciones]   `

### Opciones comunes:

*   **ps sin opciones**: Muestra los procesos asociados con la sesión actual del terminal.
    
*   **ps a**: Lista todos los procesos asociados a un terminal.
    
*   **ps aux**: Muestra todos los procesos en el sistema, incluyendo los que no están vinculados a un terminal.
    
*   **ps -C** : Filtra procesos por nombre. Ejemplo:
    

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   ps -C nano   `

**Comentario**: Este comando es ideal para identificar procesos específicos o realizar un análisis rápido del sistema.

2\. Comando top
---------------

El comando top permite monitorizar el sistema en tiempo real, proporcionando una vista dinámica de los procesos en ejecución y el uso de recursos del sistema (CPU, memoria, etc.).

### Sintaxis básica:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   top [opciones]   `

### Opciones comunes:

*   **top T**: Muestra el tiempo total de ejecución de los procesos.
    
*   **top M**: Ordena los procesos por uso de memoria.
    
*   **top P**: Ordena los procesos por uso de CPU.
    
*   **top p**: Muestra un proceso específico por su PID.
    
*   **top U** : Filtra los procesos de un usuario específico.
    
*   **top q**: Sale del comando sin confirmación.
    
*   **top k**: Permite finalizar un proceso ingresando su PID.
    

### Ejemplo:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   top -u root   `

**Comentario**: Es una herramienta clave para detectar procesos que consumen demasiados recursos.

3\. Comando htop
----------------

htop es una versión mejorada de top, con una interfaz más interactiva y amigable. Ofrece funcionalidades adicionales como filtros, búsqueda y terminación de procesos.

### Sintaxis básica:

Plain textANTLR4BashCC#CSSCoffeeScriptCMakeDartDjangoDockerEJSErlangGitGoGraphQLGroovyHTMLJavaJavaScriptJSONJSXKotlinLaTeXLessLuaMakefileMarkdownMATLABMarkupObjective-CPerlPHPPowerShell.propertiesProtocol BuffersPythonRRubySass (Sass)Sass (Scss)SchemeSQLShellSwiftSVGTSXTypeScriptWebAssemblyYAMLXML`   htop [opciones]   `

### Opciones:

*   **htop -u** : Filtra procesos de un usuario específico.
    
*   **htop --tree**: Muestra los procesos en una vista jerárquica.
    
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
    
*   atop -r archivo\_de\_registro
    

**Comentario**: atop es una herramienta esencial para monitorear sistemas de forma detallada y con la posibilidad de analizar históricos.

Qué es el PID
-------------

El **PID** (_Process ID_ o Identificador de Proceso) es un número único asignado por el sistema operativo a cada proceso en ejecución. Este identificador permite a los administradores distinguir y gestionar procesos individuales. Por ejemplo, puedes usar un PID para:

*   kill
    
*   Mostrar información de un proceso específico con top -p.
