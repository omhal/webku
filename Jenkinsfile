pipeline {
   agent any
   
   stages {
      stage('Build') {
         steps {
            sh "docker rm -f ff69cee7f397 \$(docker ps -a -q)"
            sh "docker-compose -f /var/lib/jenkins/workspace/nginx-pipeline@3/docker/docker-compose.yml up -d --build"
         }
      }
   }
}
