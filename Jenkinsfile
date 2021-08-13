def obbject = readJSON file: "test.json"

pipeline {
    agent any

    stages {
        stage('Initialize') {
            steps {
                script {
                    //map.each { entry ->
                        //stage (entry.key) {
                            //timestamps{
                            //for (key in object.element.keySet()) {
                                //echo "key=${key}"
                               // echo "value= ${object.element.get(key)}"
                           // }
                           //echo "$entry.key -> $entry.value"
                            //}
                             object.each { key, value ->
                             echo "Walked through key $key and value $value"
                            }
                        }
                    }
                }
            }
