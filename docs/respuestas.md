# Respuestas

## Preguntas de control

**¿Qué ventaja tiene registrar las dependencias del proyecto en requirements.txt en lugar de compartir la carpeta .venv?**

- Registrar las dependencias en requirements.txt es mejor que compartir la carpeta .venv porque el archivo es ligero, fácil de versionar con Git y permite que cualquier persona reconstruya el entorno en su propio sistema con python en cambio, .venv incluye archivos instalados, ejecutables y configuraciones que pueden ocupar mucho espacio y depender del sistema operativo o de rutas locales.

**¿Por qué el repositorio que tienes ahora en tu computadora no es el mismo concepto que el fork creado en GitHub?**
- El fork es una copia del repositorio original almacenada de forma remota en mi cuenta de GitHub, mientras que el repositorio que tengo en mi computadora es una copia local obtenida mediante clone. El fork permite realizar la colaboración desde GitHub y el repositorio local permite modificar y registrar los archivos desde mi computadora.

## Preguntas individuales

**79. ¿Cómo identificaste el comando necesario?**

Relacioné cada acción descrita (ej. "prepara el cambio") con el concepto de Git que le corresponde, y comprobe el resultado en VS Code o GitHub antes de continuar.

**80. Diferencia entre preparar (stage) y hacer commit**

Preparar (add) solo marca los archivos que quieres incluir en el próximo registro; el commit crea ese registro de forma permanente en el historial con un mensaje.

**81. ¿Cómo comprobar en qué rama estás?**

Con git branch (la rama activa aparece marcada con *), o viendo el nombre de la rama en la barra inferior de VS Code / el selector de ramas en GitHub.

**82. ¿Cómo saber qué archivos fueron modificados?**

Con git status, que lista los archivos modificados, nuevos o eliminados antes de prepararlos.

**83. ¿Cómo ver exactamente qué cambió dentro de un archivo?**

Con git diff, que muestra línea por línea qué se agregó o eliminó comparado con la versión anterior.

**84. ¿Por qué reconstruir .venv después de obtener un repositorio?**

Porque .venv nunca se sube a GitHub (está en .gitignore); cada quien debe crear su propio entorno virtual localmente e instalar las dependencias.

**85. Relación entre requirements.txt y .gitignore**

Son complementarios: .gitignore excluye el entorno virtual pesado (.venv/), mientras que requirements.txt sí se sube y permite reconstruir ese entorno con las dependencias exactas.

**86. ¿Por qué colaborar desde una rama y no desde main?**

Para no afectar directamente el código estable de main; la rama permite trabajar y revisar los cambios de forma aislada antes de integrarlos.

**87. ¿Por qué una solicitud de cambios no requiere un nuevo PR?**

Porque el PR está ligado a la rama, no a un commit específico; al subir nuevos commits a esa misma rama, el PR existente se actualiza automáticamente.

**88. ¿Por qué actualizar el repo local después del merge en GitHub?**

Porque el merge solo modifica el repositorio remoto; la copia local no se sincroniza sola, se necesita hacer pull para traer esos cambios a la computadora.
