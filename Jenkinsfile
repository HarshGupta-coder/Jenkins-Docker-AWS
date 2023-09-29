    pipeline {
        agent { label 'dev-node' } 
        
        stages{
            stage('Code'){
                steps {
                    git url: 'https://github.com/HarshGupta-coder/temp.git',branch: 'master'
                }
            }
            stage('Build and test'){
                steps {
                    echo 'Build and Test'
                    sh 'docker build . -t node-todo-app'
                }
            }
            stage('Login and Push Image'){
                steps {
                    echo 'Logging into dockeHub and pushing image'
                    withCredentials([usernamePassword(credentialsId:'Docker', passwordVariable:'DockerPassword', usernameVariable:'DockerUser')]){
                        sh "docker login -u ${env.DockerUser} -p ${env.DockerPassword}"
                        sh "docker tag node-todo-app:latest ${env.DockerUser}/node-todo-app:latest"
                        sh "docker push ${env.DockerUser}/node-todo-app"
                    }
                }
            }
            
            stage('Deploy'){
                steps {
                    echo 'Deploy'
                    sh 'docker-compose down && docker-compose up -d'
                }
            } 
        }
    }
