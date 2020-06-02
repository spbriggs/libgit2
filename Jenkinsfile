pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        cmakeBuild(installation: 'Autoinstall', buildDir: 'build', buildType: 'Release')
      }
    }

  }
}