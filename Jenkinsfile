pipeline {
    agent any
    stages {
        stage('Clonar código') {
            steps {
                git 'https://github.com/tu_usuario/sitio-web.git'
            }
        }
        stage('Construir imagen') {
            steps {
                sh 'docker build -t sitio-pipeline .'
            }
        }
    }
}
