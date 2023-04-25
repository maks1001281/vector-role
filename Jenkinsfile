pipeline {
    agent {
        node {
            label 'tox'
            }
      }
    stages {
        stage('git clone') {
            steps {
                sh 'git clone https://github.com/maks1001281/devops-netology.git /opt/jenkins_agent/'
    sh 'cd /opt/jenkins_agent/devops-netology/Home_work/8.4/'
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

