@Library("shared") _
pipeline{
    agent { label "vinod" }
    
    
    stages{
        
        stage("greeting"){
            steps{
                script{
                    hello()
                }
            }
        }
        
        stage("code"){
            steps{
                script{
                    codeClone("https://github.com/priyanshu-378/flask-app.git", "master")
                }
            }
            
        }
        
        stage("build"){
            steps{
                script{
                    build()
                }
            }
        }
        
        stage("push"){
            steps{
                withCredentials([usernamePassword(credentialsId:"dockerHubCred",passwordVariable:"dockerHubPassword",usernameVariable: "dockerHubUsername")]){
                    sh "docker login -u ${ env.dockerHubUsername} -p ${ env.dockerHubPassword }"
                    sh "docker tag flask-app-flask-app:latest 378priyanshu/flask-app:latest"
                    sh "docker push 378priyanshu/flask-app:latest"
                }
                echo "project deployation complete and fully automated
                
            }
        }
    }
}
