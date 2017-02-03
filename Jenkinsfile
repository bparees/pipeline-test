node('nodejs') {
  stage('build') {
    openshiftBuild(buildConfig: ''nodejs-mongodb-example, showBuildLogs: 'true')
  }
  stage('deploy') {
    openshiftDeploy(deploymentConfig: 'nodejs-mongodb-example')
  }
}

