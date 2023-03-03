pipeline{
    agent{ label 'jenkins'}
    stages{
        stage('vcs'){
            steps{
                git url: 'https://github.com/tejaswini1811/openmrs-core.git',
                    branch: 'scripted'
            } 
        }
        stage('JDK_HOME'){
            steps{
                sh 'export PATH="/usr/lib/jvm/java-11-openjdk-amd64/bin/:$PATH"'
            }
        }
        stage('package'){
            steps{
                sh ' mvn clean package'
            }
        }
    }
}