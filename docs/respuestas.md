Preguntas

 ¿Cómo identificaste el comando necesario cuando la práctica no lo proporcionó?
la verdad es que con las practicas ya se me quedaron grabados la mayoria aun asi los anoto todos los que vamos viendo en un bloc de notas por cualquier duda.

 80. ¿Qué diferencia existe entre preparar un archivo para un commit y crear el commit?
preparamos el archivo que se subira al commit.

 81. ¿Cómo puedes comprobar en qué rama estás trabajando?
con git branch

 82. ¿Cómo puedes determinar qué archivos fueron modificados antes de registrarlos?
con git status

 83. ¿Cómo puedes observar exactamente qué cambió dentro de un archivo?
con git diff

 84. ¿Por qué debe reconstruirse .venv después de obtener un repositorio?
Porque la carpeta `.venv` se ignora intencionalmente en `.gitignore` para no subirla al repositorio remoto. Cada colaborador debe generar su propio entorno virtual local según su entorno de ejecución.

 85. ¿Qué relación existe entre requirements.txt y .gitignore?
Ambos archivos se complementan para la gestión de dependencias: `.gitignore` se encarga de excluir la carpeta pesada `.venv` del repositorio, mientras que `requirements.txt` actúa como el sustituto ligero que documenta únicamente la lista y versión de los paquetes necesarios para reinstalar ese entorno en cualquier momento.

 86. ¿Por qué la colaboración se realiza desde una rama y no directamente desde main?
para checar los cambios primero

 87. ¿Por qué una solicitud de cambios no requiere crear un Pull Request nuevo?
Porque un Pull Request vincula directamente la rama remota de origen con la rama de destino. Cuando realizas correcciones y subes nuevos commits a esa misma rama mediante `git push`, el Pull Request abierto se actualiza automáticamente con el nuevo historial.

 88. Después de realizar el merge en GitHub, ¿por qué todavía es necesario actualizar el repositorio local?
Porque el *Merge* integra los cambios únicamente en la copia remota alojada en los servidores de GitHub. Para reflejar esos nuevos commits y archivos en el disco duro de la computadora local, es imprescindible ejecutar `git pull origin main`.