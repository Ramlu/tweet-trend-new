pipeline {
    agent {
        node {
            label 'maven'
        }
    }
  
    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/Ramlu/tweet-trend-new.git'      
            }        
        }
    }
}
