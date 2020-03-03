pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building ..' 
				sh "cd base-console-app \
				dotnet build ConsoleGraphTest.csproj"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
