pipeline {
    agent {
        docker {
            image 'maven:3-jdk-8-onbuild' 
            args '-v /root/.m2:/root/.m2'
            
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn install' 
            }
        }
    }
}
