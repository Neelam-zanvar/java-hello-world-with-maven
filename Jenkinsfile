pipeline{
    agent any

    tools {
         maven 'maven'
         jdk 'JDK8'
    }

    stages{
        stage('checkout'){
            steps
	         {
                // clone code from a GitHub repository
                git url: 'https://github.com/Neelam-zanvar/java-hello-world-with-maven.git'

                // Run Maven on a Unix agent.
                sh "mvn -Dmaven.test.failure.ignore=true clean test package"

             }
        }

    }
}
