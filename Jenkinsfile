pipeline {
    agent {
        node {
            label 'tox'
            }
      }
    stages {
        stage('git clone') {
            steps {
    sh 'ansible-galaxy install -r requirements.yml vector --force'
            }
        }
        stage('Tox test') {
            steps {
                dir('vector-role'){
                sh 'molecule test'
            }
   }
  }
 }
 }
