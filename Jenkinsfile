pipeline {
    agent any

    stages {
         stage('Run Playbook') {
            steps {
                ansiblePlaybook credentialsId: 'ansible-ssh', disableHostKeyChecking: true, inventory: 'dev', playbook: 'apache.yml'
            }
        }
    }
}
