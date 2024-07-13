A static website is an HTML pages served by a web server. It may include assets such as CSS, Javascripts and images.

About The Project
This project shows how to deploy a static website login page on a Docker Container.
Project Details and steps to accomplish it:
Create Static Website login pages
clone my Repo Static Login Page Files Repo

Craete a Dockerfile

Create a dockerfile Dockerfile content in the same directory of your static website login files and edit it in your favorite editor.
Use this command
touch dockerfile
To Use Nginx Web server, use the following content.
FROM nginx:alpine
COPY . /usr/share/nginx/html
Build a Docker Image
You can now create a docker image with all the created files.
Use the following command:
docker build -t sample-static-web-login:image1 .
The above command will create a Docker image with the name 'sample-static-web-login-image'
Run Docker Container
Use the just created docker image to launch a new container on your system.
Run this coomand:
docker run -d -p 80:80 sample-static-web-login:image1
You can change the host machine port to something else if the port 80 is occupied by your local machine.
The “-d” option detach the container from current shell and run in background.
Use this command to view the running container.
docker ps
Access Your Application
Access your docker host using IP address (or hostname/domain name) on port 80 to view application.
Contact
Linkedin:https://www.linkedin.com/in/elias-ibisi-007914124/

Email: yinemichael@gmail.com

Phone: +971547244788

Project Link: Project Link
https://github.com/elias-max/Website-with-Docker-sever/
References
Useful Resources And Links
Git Cheat Sheet
Docker Cheat sheet
GitHub Pages
Gitpod
Chat GPT
Nginx-docs
