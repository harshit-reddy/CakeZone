pipeline {
    agent {label 'dev'}
    tools {maven 'maven'}

    stages {
        stage('Git') {
            steps {
                git branch: 'main', url: 'https://github.com/vamsibyramala/live01.git'
            }
        }
        stage ('build') {
            steps {
                sh 'mvn clean package'
            }
        }
        
    }
}
