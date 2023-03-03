node('jenkins'){
    stage('vcs'){
        git url: 'https://github.com/tejaswini1811/openmrs-core.git',
            branch: 'scripted'
    }
    stage('JDK_HOME'){
        sh 'export PATH="/usr/lib/jvm/java-11-openjdk-amd64/bin/:$PATH"'
    }
    stage('package'){
        sh ' mvn clean package'
    }
}