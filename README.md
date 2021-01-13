docker build -t cmachadox/jenkins:v1.0 .

docker run -d  -v jenkins_vol:/var/jenkins_home -p 8080:8080 -p 50000:50000 --env JENKINS_ADMIN_ID=admin --env JENKINS_ADMIN_PASSWORD=password --name jenkins_adcc cmachadox/jenkins:v1.0

