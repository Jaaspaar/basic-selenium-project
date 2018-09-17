pipeline {
    agent {
        docker {
            image 'maven:3-alpine'
            args '-v /root/.m2:/root/.m2'
        }
    }
    stages {
        stage('Run') {
            steps {
                sh 'mvn clean verify -Pbrowser-chrome'
            }
        }
	}
}
