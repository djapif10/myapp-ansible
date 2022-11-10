pipeline{
    agent any
    stages{
       stage('Execute Ansible Playbook'){
            steps{
                ansiblePlaybook credentialsId: 'docker', disableHostKeyChecking: true, installation: 'ansible', inventory: 'dev.inv', playbook: 'apache.yml'
            }
        }
    }
}
