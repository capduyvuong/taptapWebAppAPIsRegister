pipeline {
  agent any
  stages {
    stage('run collection') {
      steps {
        sh 'docker run -t postman/newman run -h'
        sh 'docker run -v ${8c185057-1d3f-4951-958b-23bba0b1d2de}:/etc/newman --workdir /etc/newman -t postman/newman run Testing - Register flow.postman_collection.json --color off --disable-unicode'
      }
    }
  }
}
