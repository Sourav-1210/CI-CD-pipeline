pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Sourav-1210/CI-CD-pipeline.git'
            }
        }

        stage('Build Image') {
            steps {
                script {
                    sh 'docker build -t cicd-demo .'
                }
            }
        }

        stage('Remove Old Container') {
            steps {
                script {
                    try {
                        sh 'docker rm -f cicd-container'
                    } catch (Exception e) {
                        echo "No container to remove"
                    }
                }
            }
        }

        stage('Run Container') {
            steps {
                script {
                    sh 'docker run -d --name cicd-container -p 3000:3000 cicd-demo'
                }
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully! 🚀'
        }
        failure {
            echo 'Pipeline failed! ❌'
        }
    }
}
