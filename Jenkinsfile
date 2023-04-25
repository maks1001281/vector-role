pipeline {
    agent {
        node {
            label 'tox'
            }
      }
    stages {
        stage('cd work dir') {
            steps {
                sh 'cd /etc/ansible/roles/vector/'
            }
        }
        stage('Tox test') {
            steps {
                sh ',molecule test'
            }
  }
 }
}
