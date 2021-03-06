node (BK && DEV) {
    stage ('git') {
            git 'https://github.com/wakaleo/game-of-life.git'
        }
        stage('build') {
            sh 'mvn clean package'
        }
        stage('testresults') {
            junit 'gameoflife-web/sureire-reports/*.xml'
        }
}