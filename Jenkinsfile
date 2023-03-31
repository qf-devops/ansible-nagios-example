pipeline {
    agent { label 'ansible-label' }
    stages {
        stage('clone') {
            steps { 
                checkout scm
            } 
        }
        stage('ansible') {
            steps { 
                sh 'sudo -i'
                sh 'whoami'
                sh 'ansible-playbook -i hosts install/nagios.yml -b'
            } 
        }
    }
}
