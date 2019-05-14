pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                echo 'Starting checkout...'
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'LocalBranch', localBranch: 'master']], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/Romanope/curso-jenkins.git']]])
            }
        }
    }
}