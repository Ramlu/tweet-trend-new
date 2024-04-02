pipeline {
    agent {
        node {
            label 'maven'
        }
    }
    environment {
        PATH = "/opt/apache-maven-3.9.6/bin:$PATH"
    }
    
    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/Ramlu/tweet-trend-new.git'      
            }        
        }
        stage('Build') {
            steps {
                sh 'mvn clean deploy -Dmaven.test.skip=true'
            }
        }
    }
}
