pipeline {
    agent {
        docker {
            image 'maven:3-alpine' 
            args '-v /suj1982/.m2:/suj1982/.m2' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
