pipeline {
  agent any
  stages {
    stage('run collection') {
      steps {
        sh 'docker run -t postman/newman run -h'
        sh 'docker run -v ${https://taptapproject.postman.co/workspace/RAMBUTAN---Web-App~8c185057-1d3f-4951-958b-23bba0b1d2de/collection/17542940-4fdf1a51-ac7e-4db7-bd36-7170dd5f5d35?action=share&creator=17542940&active-environment=20479915-f50a357d-6bdd-401b-b842-8fd87756d360}:/etc/newman --workdir /etc/newman -t postman/newman run Testing - Register flow.postman_collection.json --color off --disable-unicode'
      }
    }
  }
}
