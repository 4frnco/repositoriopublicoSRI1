# repositoriopublicoSRI1

1. **¿Cómo descargar y comprobar que una imagen está en tu equipo?**  
   Ejecuta `docker pull ubuntu` y verifica con `docker images`. Asegúrate de que tienes conexión a Internet antes de realizar la descarga.

2. **¿Cómo crear un contenedor sin nombre?**  
   Usa `docker run -d ubuntu` y verifica el nombre con `docker ps`. Recuerda que al no asignarle un nombre, Docker generará uno automáticamente.

3. **¿Cómo crear un contenedor con el nombre 'u1'?**  
   Ejecuta `docker run -d --name u1 ubuntu` y accede con `docker exec -it u1 bash`. Esto te permitirá interactuar con el contenedor de manera efectiva.

4. **¿Cómo comprobar la IP y hacer ping a Google?**  
   Usa `ip addr show` para obtener la IP y `ping google.com` para verificar la conectividad a Internet.

5. **¿Cómo crear un contenedor con el nombre 'bono'?**  
   Crea el contenedor con `docker run -d --name bono ubuntu`. Para ping entre contenedores, primero conecta ambos a una red: ejecuta `docker network create mynet`, luego `docker network connect mynet u1` y `docker network connect mynet bono`. Haz ping desde u1 a bono con `docker exec -it u1 ping bono`. Asegúrate de que ambos contenedores estén en ejecución.

6. **¿Qué sucede si cierras las terminales?**  
   Ciérralos en modo -d y verifica su estado con `docker ps`. Si deseas detener un contenedor, utiliza `docker stop <nombre_contenedor>`.

7. **¿Cuánta memoria ocupaste en el disco duro?**  
   Usa `docker system df` para calcular la memoria ocupada. Esto te dará un resumen del uso de espacio en disco por imágenes, contenedores y volúmenes.

8. **¿Cuánta RAM ocupan los contenedores?**  
   Ejecuta `docker stats` para monitorear la RAM. Este comando proporciona información en tiempo real sobre el uso de recursos de cada contenedor.

9. **¿Cómo hiciste para clonar el repositorio?**  
   Ejecuta `git clone https://github.com/tu-usuario/docker-task.git`. Asegúrate de que la URL sea correcta y de que tienes los permisos necesarios.

10. **¿Cómo añades el archivo readme2.md?**  
    Usa `git add readme2.md` para añadir el archivo al índice de git. Asegúrate de que el archivo esté en la carpeta del repositorio.

11. **¿Cuáles son los pasos para subir el archivo que estás editando y el archivo readme2.md?**  
    Haz commit con `git commit -m "Añadir archivos README.md y readme2.md"` y push con `git push origin main`. Verifica que no haya conflictos antes de hacer push.

12. **¿Cómo comprobarías que existen diferencias entre tu repositorio local y el remoto?**  
    Usa `git fetch` y `git diff origin/main` para verificar diferencias entre local y remoto. Esto te ayudará a asegurarte de que estás al día con los cambios en el repositorio remoto.

![Carita feliz]([https://pixabay.com/get/g17b5f3968ed7cf9c1e9050a63af5e5e8c3c6cc3e96457cdccabc17cb7dbbe2b1_640.png](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.redbubble.com%2Fes%2Fshop%2Fcarita%2Bfeliz%2Bemoji%2Bstickers&psig=AOvVaw204rDVykM-CddjZm5_WwFr&ust=1727895968981000&source=images&cd=vfe&opi=89978449&ved=0CBEQjRxqFwoTCJik85zw7YgDFQAAAAAdAAAAABAE))


