pipeline{
    agent any
    stages{
        stage('clean old'){
           steps{
            sh '/opt/maven/bin/mvn clean'
        } 
        }
        
        stage('maven install'){
            steps {
                sh '/opt/maven/bin/mvn install'
            }
        }
        stage('package artifact'){
            steps {
                sh '/opt/maven/bin/mvn package'
            }
        }
    }
}
