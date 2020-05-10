node{
    stage('GIT'){
        git 'https://github.com/resourceelabb/BuildPractice.git'
    }
    stage('Package'){
        sh 'mvn package'
    }
    stage('ArchiveArtifacts'){
         archiveArtifacts 'gameoflife-web/target/*.war'
    }
    stage('Testreport'){
        junit 'gameoflife-web/target/surefire-reports/*.xml'
    }

}
