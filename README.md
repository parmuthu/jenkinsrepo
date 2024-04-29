Steps for creating docker image
  1. Run as mvn clen package or maven install to generate the packaged .jar or .war file
  2. place the Dockerfile in the project's root folder
  3. open the project folder in the command prompt,
  4. Enter the command, docker build -t "imagename you want" .
  5. execute, docker images to verify the image created
  6. to run, docker container run --name "containername"  "imagname"
  7. You application will run.

To push docker image to docker hub,
1. Create account in docker hub.
2. Create a repository

From the project folder, execute the following commands.   

# Log in to Docker Hub
docker login

# Tag your local Docker image
docker tag local_image_name:tag docker_hub_username/repository_name:tag

# Push the tagged image to Docker Hub
docker push docker_hub_username/repository_name:tag
