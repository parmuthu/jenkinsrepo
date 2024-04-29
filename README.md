Steps for creating docker image
  1. Run as mvn clen package or maven install to generate the packaged .jar or .war file
  2. place the Dockerfile in the project's root folder
  3. open the project folder in the command prompt,
  4. Enter the command, docker build -t "imagename you want" .
  5. execute, docker images to verify the image created
  6. to run, docker container run --name "containername"  "imagname"
  7. You application will run.
