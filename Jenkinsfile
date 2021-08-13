def obbject = ""

pipeline {
    agent any
    
    stages {
        stage('Initialize') {
            steps {
                script {
                        sh 'ls'
                        object= readJSON file: 'test.json', text: ''
                        echo object["a"]
                       // object.each { key, value ->
                        //echo "$key = $value"
                        
                       }
                      }
                    }
                  }
                }
              //}
