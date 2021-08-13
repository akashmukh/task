def obbject = ""
def name = ""
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
                        //echo object["a"]
                        object.each { key, value ->
                            name = $key
                            if (params.Choice == $name) {
                                echo $value    
                            }
                        //echo "$key = $value"      
                       }
                      }
                    }
                  }
                }
               }
