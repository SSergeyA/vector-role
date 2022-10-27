pipeline {
    agent {
        label 'centos'
    }

   

    stages {
        stage('Checkout SCM') {
            steps {
                git branch: 'main', credentialsId: '04701acb-e269-486e-84fa-ac067a79f127', url: 'git@github.com:SSergeyA/vector-role.git'
            }
        }
        stage('Molecule') {
            steps {
             sh 'molecule test'   
            }

            
            
        }
    }
}
