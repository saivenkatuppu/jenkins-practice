pipeline {
  agent { 
        label 'AGENT-1'
    
}
    stages {
        stage('Build') {
            steps {
               script{
                echo "buildong"
               }
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
    post { 
        always { 
            echo 'I will always say Hello again!'
            deleteDir()
        }
        success{
            echo" hello success"
        }
        failure{
            echo"hello its failure"
        }
    }
}
  