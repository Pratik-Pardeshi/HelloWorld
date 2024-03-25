pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout code from Git repository
                git 'https://github.com/Pratik-Pardeshi/HelloWorld.git'
            }
        }

        stage('Build') {
            steps {
                // Build the Maven project
                sh 'mvn clean package'
            }
        }

        stage('Deploy') {
            steps {
                // Deploy the code to a web server
                // This step depends on your deployment setup
                // You might need to use SSH, FTP, or any other method to deploy
                // For example, if deploying to Tomcat:
                sh 'cp target/your_project.war /path/to/tomcat/webapps/'
            }
        }
    }
}
