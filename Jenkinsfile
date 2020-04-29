node('UBUNTU'){
    stage('GIT'){
        git 'https://github.com/resourceelabb/BuildPractice.git'
    }
    stage('Package'){
        sh 'mvn package'
    }
}