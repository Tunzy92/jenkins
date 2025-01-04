pipeline {
    agent any 
    stages {
        stage ('docker image') {
            steps {
                script {
                    img = 'httpd:2.4-alpine'
                    docker.image("${img}").run('-d -p 80:80')
                }
            }
        }
    }
}
