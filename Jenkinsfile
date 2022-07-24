pipeline {
   agent any 
   stages {
        stage("build") {
           steps {
             echo "build stage"
            }
        }
        stage("test") {
           when {
              expression {
                 BRANCH_NAME == 'DEV' || BRANCH_NAME == 'master' 
              }
           }
           steps {
             echo "test stage"
            }
        }
        stage("deploy")
           steps {
             echo "deploy stage"
             }
        }
    }
post {
   always {
      
   }
   success {
    }
  }
}
