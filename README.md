<h1 align="center">Hi 👋, We're Pandoe</h1>
<h3 align="center">Bussiness Idea, Just For You</h3>

1. run the model program which already in [model](https://github.com/C241-PS488/pandoe-ml)
2. save the model to tensorflow model
3. store the model to cloud storage
4. download the web service which is already in [web service](https://github.com/C241-PS488/pandoe-web-service)
5. build the code to docker image using this ```docker build -t gcr.io/project-id-gcp/image-name:version .```
6. push the image to artifact registry ```docker push gcr.io/project-id-gcp/image-name:version```
7. setup cloud sql instances in google cloud platform and choose mysql for database
8. create the name of database
9. open cloud run service, choose previously pushed image from artifact registry
10. set the env variables
   ```
   DATABASE_URL = "mysql://root:passwordofyourcloudsqlinstances:3306/yourdatabasename?socket=/cloudsql/instancesconnectionname"
   PORT = 8080 //yours
   JWT_SECRET = "yours"
   MODEL_URL = "yours"
   GOOGLE_APPLICATION_CREDENTIALS = "yours"
   ```
11. deploy
12. integrate the api to mobile app
13. run the app.
