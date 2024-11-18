pipeline {
    agent any

    stages {
        stage('git clone') {
            steps {
                git branch: 'main', url: 'https://github.com/LakshyaGulenia/donation-flask.git'
            }
        }
        stage('build') {
            steps {
                sh 'docker compose down'
                sh 'docker compose up -d'
            }
        }
        // stage('git clone2') {
        //     steps {
        //         echo 'Hello World'
        //     }
        // }
        
    }
}
