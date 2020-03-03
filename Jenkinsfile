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
                echo 'Deploying.....'
		sh "sudo apt-get update"
		sh "sudo apt-get install docker-ce docker-ce-cli containerd.io"
            }
        }
    }
}
