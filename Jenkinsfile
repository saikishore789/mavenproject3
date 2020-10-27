pipeline {
  agent any
  stages {
    stage('gitcode') {
      steps {
        git(url: 'https://github.com/saikishore789/mavenproject3.git', branch: 'master', changelog: true, poll: true)
      }
    }

    stage('maven') {
      steps {
        bat 'mvn package'
      }
    }

  }
}