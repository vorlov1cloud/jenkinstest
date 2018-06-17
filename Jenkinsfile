pipeline {
  agent any
  stages {
    stage('test shell') {
      parallel {
        stage('test shell') {
          steps {
            sh 'echo OK && mkdir /root/sex'
            sleep 10
          }
        }
        stage('test shel 2') {
          steps {
            sh 'echo sex2 && mkdir /root/sex2'
          }
        }
      }
    }
    stage('mv shell') {
      steps {
        sh 'mv /root/sex /root/sex2/ && echo moved'
      }
    }
    stage('end') {
      steps {
        echo 'sosite huy'
      }
    }
  }
}