pipeline {
    agent any

    stages {

        stage('Construir imagen') {
            steps {
                sh 'docker build -t mi-sitio-web .'
            }
        }

        stage('Ejecutar contenedor') {
            steps {
                sh 'docker run -d -p 8081:80 mi-sitio-web'
            }
        }
    }
}
