pipeline {
  agent any
  stages {
    stage('clone') {
      steps {
        git 'https://github.com/MahmoudKammoun/kernel-linux.git'
      }
    }
    stage('Configure') {
      steps {
         sh label: '', script: 'cp -v /boot/config-$(uname -r) .config'
      }
    }
    stage('Configuring') {
      steps {
         sh label: '', script: 'make config'
      }
    }
    }
    }
