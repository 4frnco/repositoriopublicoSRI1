# repositoriopublicoSRI1

Descargar imagen: Ejecuta docker pull ubuntu y verifica con docker images.

Crear contenedor sin nombre: Usa docker run -d ubuntu y verifica el nombre con docker ps.

Crear contenedor 'u1': Ejecuta docker run -d --name u1 ubuntu y accede con docker exec -it u1 bash.

Comprobar IP y hacer ping a Google: Usa ip addr show para obtener la IP y ping google.com para hacer ping.

Crear contenedor 'bono': Crea el contenedor con docker run -d --name bono ubuntu. Para ping entre contenedores, conecta ambos a una red: docker network create mynet, luego docker network connect mynet u1 y docker network connect mynet bono. Haz ping desde u1 a bono con docker exec -it u1 ping bono.

Estado de los contenedores: Ciérralos en modo -d y verifica con docker ps.

Memoria en disco: Usa docker system df para calcular la memoria ocupada.

RAM de los contenedores: Ejecuta docker stats para monitorear la RAM.

Clonar el repositorio: Ejecuta git clone https://github.com/tu-usuario/docker-task.git.

Añadir readme2.md: Usa git add readme2.md.

Subir archivos al repositorio remoto: Haz commit con git commit -m "Añadir archivos README.md y readme2.md" y push con git push origin main.

Comprobar diferencias: Usa git fetch y git diff origin/main para verificar diferencias entre local y remoto.
