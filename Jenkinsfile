pipeline {
  agent any
  stages {
    stage('Source') {
      steps {
        git 'https://github.com/MahmoudKammoun/kernel-linux.git'
      }
    }
    stage('Configure the Linux kernel features and modules') {
      steps {
         sh label: '', script: 'cp -v /boot/config-$(uname -r) .config'
      }
    }
    stage('Install the required compilers and other tools') {
      steps {
         sh label: '', script: 'make -j 4'
      }
    }
    }
    }
