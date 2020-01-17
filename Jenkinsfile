pipeline {
   agent any
   
   stages {
      stage('Build') {
         steps {
            sh "docker rm -f \$(docker ps -a -q)"
            //sh "docker-compose up /var/lib/jenkins/workspace/nginx/docker/docker-compose.yml -d --build"
            sh "docker-compose up -d --build\n"
         }
      }
   }
}
