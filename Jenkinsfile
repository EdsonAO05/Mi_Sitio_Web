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
                sh '''
                docker rm -f mi-sitio-web || true
                docker run -d --name mi-sitio-web -p 8090:80 mi-sitio-web
                '''
            }
        }
    }
}

