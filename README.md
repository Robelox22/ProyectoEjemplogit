# Práctica 1: introducción a Git

## Descripción
Este proyecto es una introducción a los comandos básicos de Git, La práctica está diseñada para a crear y gestionar un repositorio en Git, realizar commits, configurar archivos que deben ser ignorados en el control de versiones y subir el proyecto a un repositorio remoto en GitHub. El programa HolaMundo.py es un ejemplo simple en Python que imprime un mensaje en la consola, lo que permite practicar comandos de Git mientras se trabaja en un archivo de código.

El objetivo principal de esta práctica es comprender cómo se realizan los cambios en el código, cómo hacer un seguimiento de versiones a través de commits y cómo interactuar con un repositorio remoto. Esto nos ayuda para el manejo de proyectos colaborativos.

## Instrucciones de uso
Este programa, HolaMundo.py, está diseñado para ejecutarse en Python y simplemente imprime un mensaje en la consola. Es ideal para verificar que Git rastrea correctamente los cambios y permite probar las funciones básicas de un control de versiones en un archivo de código.

Para ejecutar el programa, sigue estos pasos:

1. Abre Git Bash.
2. Navega a la carpeta del proyecto donde se encuentra HolaMundo.py, por ejemplo: cd ~/Desktop/ProyectoEjemploGit
3. Ejecuta el programa con el siguiente comando: python HolaMundo.py
4. Deberías ver el mensaje "Hola Mundo" . Esto indica que el programa se ejecutó correctamente y que el entorno de Python está configurado.

## Comandos utilizados
- mkdir ProyectoEjemploGit                                        # Crear la carpeta del proyecto
- cd ProyectoEjemploGit                                           # Entrar en la carpeta del proyecto
- git init                                                        # Inicializar el repositorio de Git
- echo 'print("Hola Mundo")' > HolaMundo.py                       # Crear el archivo HolaMundo.py
- git add HolaMundo.py                                            # Añadir el archivo al área de preparación
- git commit -m "Se agregó el programa de Hola Mundo en Python"   # Primer commit
- git status                                #                     # Verificar el estado
- git remote add origin "URL"                                     # Conectar a GitHub
- git push -u origin master                                       # Subir los commits al repositorio remoto




## Notas sobre el archivo .gitignore
### Archivos ignorados
La instrucción *.log dentro de .gitignore le dice a Git que ignore todos los archivos con extensión .log. Esto es útil para omitir archivos de registro o de depuración que suelen ser temporales y que, en un proyecto real, solo ocuparían espacio innecesario en el repositorio.

### Verificación del .gitignore
Para verificar que Git esté ignorando correctamente el archivo debug.log, puedes utilizar el comando git status, que mostrará los archivos rastreados y no rastreados. Si debug.log no aparece en la lista de archivos no rastreados, significa que el .gitignore está funcionando correctamente. Además, al subir el proyecto a GitHub, este archivo no debería aparecer, confirmando que se ha ignorado en el control de versiones.







