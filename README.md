CMD - docker-compose run anup_web django-admin startproject core .
Error:
D:\Docs_django_docker>docker-compose run anup_web django-admin startproject composeexample .
Creating docs_django_docker_anup_web_run ... error

ERROR: for docs_django_docker_anup_web_run  Cannot create container for service anup_web: invalid volume specification: '/d/Docs_django_docker/code:/code:rw'    

ERROR: for anup_web  Cannot create container for service anup_web: invalid volume specification: '/d/Docs_django_docker/code:/code:rw'
ERROR: Encountered errors while bringing up the project.



FIX:
On the docker in the tray, right click —-> Switch to Linux Containers

This may throw another error - ”Not enough memory “. To resolve this, restart docker 

Go to settings of docker —> Resources —-> File Sharing 
Add the directory from where you’re running the project. 

Now rerun the command in the terminal 
