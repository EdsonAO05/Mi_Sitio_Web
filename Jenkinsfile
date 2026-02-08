pipeline {
    agent any
    stages {
        stage('Clonar código') {
            steps {
                git 'https://github.com/EdsonAO05/Mi_Sitio_Web.git'
            }
        }
        stage('Construir imagen') {
            steps {
                sh 'docker build -t sitio-pipeline .'
            }
        }
    }
}
