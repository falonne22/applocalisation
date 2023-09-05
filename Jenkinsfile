pipeline{
    tools{
        maven 'M2_HOME'
    }
    agent any
    stages{
        stage('clean old'){
           steps{
            sh 'mvn clean'
        } 
        }
        
        stage('maven install'){
            steps {
                sh 'mvn install'
            }
        }
        stage('package artifact'){
            steps {
                sh 'mvn package'
            }
        }
    }
}
