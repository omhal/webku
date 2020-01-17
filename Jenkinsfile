pipeline {
   agent any
   
   stages {
      stage('Build') {
         steps {
            sh "docker rm -f \$(docker ps -a -q)"
            sh "docker-compose -f /var/lib/jenkins/workspace/nginx/docker/docker-compose.yml up --build"
         }
      }
   }
}
