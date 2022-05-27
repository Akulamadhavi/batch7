pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'git clone'
                git 'https://github.com/wakaleo/game-of-life.git'
            }
        }
        stage('building artifact') {
            steps {
                echo 'building artifart using maven'
                sh 'mvn clean install'
            }
        }
   }
}
