pipeline {
  agent {
    node {
      label 'mac'
    }

  }
  stages {
    stage('build') {
      steps {
        cmakeBuild(installation: 'Autoinstall', buildDir: 'build', buildType: 'Release')
      }
    }

  }
}