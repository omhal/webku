pipeline {
   agent any
   
   stages {
      stage('Build') {
         steps {
            sh "docker rm -f \$(docker ps -a -q)"
            sh "docker-compose /var/lib/jenkins/workspace/nginx/docker/docker-compose.yml up -d --build"
         }
      }
   }
}
