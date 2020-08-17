pipeline {
  agent any
  stages {
    stage('Source') {
      steps {
        git 'https://github.com/MahmoudKammoun/kernel-linux.git'
      }
    }
    stage('Compile') {
      steps {
         sh label: '', script: 'cp -v /boot/config-$(uname -r) .config'
      }
    }
    }
    }
