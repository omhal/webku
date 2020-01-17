import jenkins.model.*
jenkins = Jenkins.instance

node{

    stage(‘Build’) {

      sh ‘docker-compose -f /var/lib/jenkins/workspace/nginx/docker/docker-compose.yml up --build’
    }

}
