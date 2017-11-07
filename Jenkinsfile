pipeline {
    agent any
    stages {
        stage('build Success'){
            steps {

             echo "will succeed"

             sh 'node app'
             sh 'mocha test/success.js'
            }


           }

        stage('build Failure'){
            steps {
             echo "will fail"

             sh 'node -v'
             sh 'npm install'
             sh 'node app'
             sh 'mocha test/error.js'
            }

         }
    }
}