node('master') {
  stage('Checkout') {
    deleteDir()
    git credentialsId: '1d7da0f5-06cb-4649-ac42-90b68e04f7e4', url: 'git@github.com:beeva-sergiomarcos/course-cicd.git'
  }

  stage('Test') {
    sh './simplehttpserver/tests/unittests.sh ./simplehttpserver/'
}
}
