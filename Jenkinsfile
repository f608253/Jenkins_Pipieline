pipeline {
        agent any
        stages {
              stage ('Compile stage') {
                    steps {
                          sh 'maven clean compile'
                             
                        }
                  }

               stage ('Testing stage') {
                    steps {
                          sh 'mvn test'
                             
                        }
                  }

               stage ('Deploy stage') {
                    steps {
                          sh 'mvn deploy'
                             
                        }
                  }
        }
}
