# le-basic-nginx-image

Basic Docker image to run nginx servers. Also a boilerplate for laravel server

To properly run image type in terminal:

Enter project folder:

`cd [path-to-project]`

Build image and delete cache
`docker build --no-cache -t [image-name] .`

Run image and map port 80 to container, mount `src` folder to container server public directory

`docker run --rm -p 80:80 -v [path-to-project]/src:/var/www/html/public [image-name]`

While running container all changes in the src directory will be reflected on web server. 