pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning Repository...'
                git branch: 'main', url: 'https://github.com/FETAKE/DEMOSPRING.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
                sh './mvnw clean package' // or 'mvn clean package' if not using wrapper
            }
        }
    }
}
