@Library('Shared')_
pipeline{
    agent any 
    
    stages{
        stage("Code clone"){
            steps{
                sh "whoami"
            clone("https://github.com/786israhul-art/django-notes-app.git","main")
            }
        }
        stage("Code Build"){
            steps{
            //dockerbuild("notes-app","latest")
            echo "docker build"
            }
        }
        stage("Push to DockerHub"){
            steps{
                //echo " dockerpush("dockerHubCreds","notes-app","latest") "
                echo "docker push"
            }
        }
        stage("Deploy"){
            steps{
                echo "deploy()"
            }
        }
        
    }
}
