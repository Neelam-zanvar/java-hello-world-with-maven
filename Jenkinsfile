pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World from master branch'
                logstashSend failBuild: true, maxLines: -1
            }
        }
    }
}


