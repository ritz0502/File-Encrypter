pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/ritz0502/File-Encrypter.git'
            }
        }

        stage('Build') {
            steps {
                sh '''
                echo "Building Java Project..."
                cd "Password Protection"
                mkdir -p build
                javac -d build src/*.java
                echo "Build Successful"
                '''
            }
        }

        stage('Test') {
            steps {
                sh '''
                echo "Running Tests..."
                cd "Password Protection"
                echo "No automated tests configured"
                '''
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                echo "Deploy Stage (Simulation)"
                echo "Application Ready"
                '''
            }
        }

    }
}
