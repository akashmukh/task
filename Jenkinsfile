def obbject = ""
def val= ""

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
                        object= readJSON file: 'test.json', text: ''
                        object.each { key, value ->
                          if (params.Choice == "$key") {
                                echo "$value"
                                val= "$value"
                          }
                        //echo "$key = $value"      
                       }
                      }
                    }
                  }
        stage('PRINT') {
           steps {
               script {
                   echo "$val"
                 }
               }
             }
           }
         }
