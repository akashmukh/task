def obbject = ""

pipeline {
    agent any

    parameters {
        string(name: 'Choice',  defaultValue: '',  description: '')
        
    }
    stages {
        stage('Initialize') {
            steps {
                script {
                        sh 'ls'
                        object= readJSON file: 'test.json', text: '{ "key": null, "a": "b" }'
                        assert object['key'] == null
                        object.each { key, value ->
                          if (params.Choice == "$key") {
                                echo "$value"
                          }
                        //echo "$key = $value"      
                       }
                      }
                    }
                  }
        stage('PRINT') {
           steps {
               script {
                   echo "$value"
                 }
               }
             }
           }
         }
