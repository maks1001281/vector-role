pipeline {
    agent {
        node {
            label 'tox'
            }
      }
    stages {
        stage('Ansible install role') {
            steps {
    sh 'ansible-galaxy install -r requirements.yml vector --force'
            }
        }
        stage('Molecule test podman') {
            steps {
                dir('vector'){
                sh 'molecule test'
            }
   }
  }
 }
 }
