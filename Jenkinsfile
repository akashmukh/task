def obbject = ""

pipeline {
    agent any

    
    stages {
        stage('Initialize') {
            steps {
                script {
                        sh 'ls'
                        object= readJSON file: 'test.json', text: ''
                        object.each { key, value ->
                                echo "$key"
                                echo "$value"
                                $key= "$value"      
                       }
                        echo object.a
                      }
                    }
                  }
        stage('PRINT') {
           steps {
               script {
                   echo object.b
                 }
               }
             }
           }
         }
