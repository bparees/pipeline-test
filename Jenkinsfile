node('nodejs') {
  stage('build') {
    sh 'echo HELLO world UPDATE'
    openshiftBuild(buildConfig: 'nodejs-mongodb-example', showBuildLogs: 'true')
  }
  stage('deploy') {
    openshiftDeploy(deploymentConfig: 'nodejs-mongodb-example')
  }
}

