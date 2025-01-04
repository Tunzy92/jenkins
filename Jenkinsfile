pipeline {
    agent any
    stages {
        stage('Run Docker') {
            steps {
                script {
                    img = 'nginx:1.27.3-alpine'
                    docker.image("${img}").run('-d -p 8080:80')
                }
            }
        }
    }
}

