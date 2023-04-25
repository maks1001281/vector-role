pipeline {
    agent {
        node {
            label 'tox'
            }
      }
    stages {
        stage('git clone') {
            steps {
    sh 'git clone https://github.com/maks1001281/devops-netology.git $HOME/jenkins/'
    sh 'cd $HOME/jenkins/Home_work/8.4
    sh 'ansible-galaxy install -r requirements.yml vector --force'
            }
        }
        stage('Tox test') {
            steps {
                sh 'tox'
            }
  }
 }
}

