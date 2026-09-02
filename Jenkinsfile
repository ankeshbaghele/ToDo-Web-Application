
 pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build Frontend Image') {
            steps {
                sh 'docker build -t ankeshbaghele/todo-app:latest .'
            }
        }

        stage('Build Backend Image') {
            steps {
                sh 'docker build -t ankeshbaghele/todo-backend:latest ./backend'
            }
        }

        stage('Push Images to Docker Hub') {
            steps {
                withCredentials([
                    usernamePassword(
                        credentialsId: 'dockerhub',
                        usernameVariable: 'DOCKER_USERNAME',
                        passwordVariable: 'DOCKER_PASSWORD'
                    )
                ]) {
                    sh '''
                        echo "$DOCKER_PASSWORD" | docker login -u "$DOCKER_USERNAME" --password-stdin

                        docker push ankeshbaghele/todo-app:latest
                        docker push ankeshbaghele/todo-backend:latest
                    '''
                }
            }
        }

        stage('Deploy Frontend') {
            steps {
                sh '''
                    docker rm -f todo-container || true
                    docker pull ankeshbaghele/todo-app:latest
                    docker run -d \
                        -p 4173:4173 \
                        --name todo-container \
                        ankeshbaghele/todo-app:latest
                '''
            }
        }

        stage('Deploy Backend') {
            steps {
                sh '''
                    docker rm -f todo-backend || true
                    docker pull ankeshbaghele/todo-backend:latest
                    docker run -d \
                        --env-file /mnt/c/Users/ankes/todo/ToDo-Web-Application/backend/.env \
                        -p 5000:5000 \
                        --name todo-backend \
                        ankeshbaghele/todo-backend:latest
                '''
            }
        }
    }
}
