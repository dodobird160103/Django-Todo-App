# Django-Todo
 Containerization and CI/CD Pipelines of a Python Application. 
 
 <h1> How it Works</h1>
 This project I have created represents the concepts of container orchestration and CI/CD pipelines that I have learnt.
 Developer will commit the code, the commit will be transfered to Gitlab using Github webhooks. Gitlab will recognise
 the changes and will start executing the CI/CD Pipelines. There are multiple jobs in CI/CD pipelines for automation purposes. 
 The CI/CD automation will create a docker image and push to farhan1471/todo_app repository on docker hub. From there it will be
 a docker container would run on a gitlab runner for testing the application.
 <br></br>
 <ul>
  <li><b>Test: </b><p>This job will run tests to verify integrity of changes made in code.</p></li>
  <li><b>Build: </b><p>This job will make a docker image using Dockerfile and push it to docker hub repository.</p></li>
  <li><b>Deploy: </b><p>This job will pull the image from docker hub and will use the runner image as docker to
   run the application image inside docker container.</p></li>
 </ul>

 
