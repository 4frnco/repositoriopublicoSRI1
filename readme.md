# repositoriopublicoSRI1

Descargar imagen: Ejecuta docker pull ubuntu y verifica con docker images. Asegúrate de que tienes conexión a Internet antes de realizar la descarga.

Crear contenedor sin nombre: Usa docker run -d ubuntu y verifica el nombre con docker ps. Recuerda que al no asignarle un nombre, Docker generará uno automáticamente.

Crear contenedor 'u1': Ejecuta docker run -d --name u1 ubuntu y accede con docker exec -it u1 bash. Esto te permitirá interactuar con el contenedor de manera efectiva.

Comprobar IP y hacer ping a Google: Usa ip addr show para obtener la IP y ping google.com para verificar la conectividad a Internet.

Crear contenedor 'bono': Crea el contenedor con docker run -d --name bono ubuntu. Para ping entre contenedores, primero conecta ambos a una red: ejecuta docker network create mynet, luego docker network connect mynet u1 y docker network connect mynet bono. Haz ping desde u1 a bono con docker exec -it u1 ping bono. Asegúrate de que ambos contenedores estén en ejecución.

Estado de los contenedores: Ciérralos en modo -d y verifica su estado con docker ps. Si deseas detener un contenedor, utiliza docker stop <nombre_contenedor>.

Memoria en disco: Usa docker system df para calcular la memoria ocupada. Esto te dará un resumen del uso de espacio en disco por imágenes, contenedores y volúmenes.

RAM de los contenedores: Ejecuta docker stats para monitorear la RAM. Este comando proporciona información en tiempo real sobre el uso de recursos de cada contenedor.

Clonar el repositorio: Ejecuta git clone https://github.com/tu-usuario/docker-task.git. Asegúrate de que la URL sea correcta y de que tienes los permisos necesarios.

Añadir readme2.md: Usa git add readme2.md para añadir el archivo al índice de git. Asegúrate de que el archivo esté en la carpeta del repositorio.

Subir archivos al repositorio remoto: Haz commit con git commit -m "Añadir archivos README.md y readme2.md" y push con git push origin main. Verifica que no haya conflictos antes de hacer push.

Comprobar diferencias: Usa git fetch y git diff origin/main para verificar diferencias entre local y remoto. Esto te ayudará a asegurarte de que estás al día con los cambios en el repositorio remoto.
