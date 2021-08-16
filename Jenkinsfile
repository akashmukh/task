def obbject = ""

pipeline {
    agent any

    object= readJSON file: 'test.json', text: ''
    object.each { key, value ->
    parameters {
        string(name: 'Choice',  defaultValue: '',  description: '')
        
    }
    stages {
        stage('Initialize') {
            steps {
                script {
                        sh 'ls'
                        //object= readJSON file: 'test.json', text: ''
                       // object.each { key, value ->
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
