node('jenkins'){
    stage('vcs'){
        git url: 'https://github.com/tejaswini1811/openmrs-core.git',
            branch: 'scripted'
    }
    stage('package'){
        sh 'cd openmrs-core && mvn clean package'
    }
}