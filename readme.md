Build the container:
docker build -t python-hello-world:latest .
https://docs.docker.com/engine/reference/commandline/build/

Run the Windows container locally:
docker run -dp 5000:5000 --name phw python-hello-world:latest
https://docs.docker.com/engine/reference/commandline/run/

Save the image to a file:
docker save python-hello-world:latest -o image.tar
https://docs.docker.com/engine/reference/commandline/image_save/
Note: It's over 3GB

Load the image from a file:
docker load -i image.tar
https://docs.docker.com/engine/reference/commandline/image_load/