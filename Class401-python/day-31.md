# Reading - Django REST Framework & Docker
## A Beginner's Guide to Docker
* A way to isolate and run entire applications
  * Doesn't matter if youre using Mac, Windows, or Linux, environment is isolated

### Linux Containers
* Mini Virtual Machines
* Take away all the excess resources that a Virtual Machine has but allows similar functionality

### Containers vs Virtual Environments
* Virtual environments utilize Python software packages that are installed locally
* You need to have that version of Python installed on your device in order to use the virtual environment
* You can't run a production database or other services within a VE

### Install Docker
* Download Docker, check installation below
* `docker --verions`
* `docker-compose --version`
* couldnt get hello-world to run

### Images and Containers
* Image: A snapshot in time of what a project contains
* Container: A running instance of the image
* When we run `hello-world` we use an official Docker image, did not create our own image
* You can create your own image using a `Dockerfile`
* Use `docker-compsose.yml` to run containers

Analogy:
* `Dockerfile` is the recipe for the cake
* Image is a snapshot of the recipe at a given time
* `docker-compose.yml` says how to ake the cake
* Container is the actual, baked cake

### Images
Create an image and container just for Python
* `touch Dockerfile`
* `FROM python:3.7-alpine`

### Image Builds
* `docker image build .`

### Image Layers
* All images are made up of one or more image layers
* Base layer is usually Linux
* Image layering exists so:
  * Each image layer is immutable, ensuring consistency for multiple devs
  * Performance
