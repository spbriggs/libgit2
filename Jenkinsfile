pipeline {
  agent {
    node {
      label 'mac'
    }

  }
  stages {
    stage('build') {
      steps {
        cmakeBuild(installation: 'Autoinstall', buildDir: 'build', buildType: 'Release', cleanBuild: true, cmakeArgs: '--build')
        cmake(installation: 'Autoinstall', arguments: '--build .', workingDir: 'build')
      }
    }

  }
}