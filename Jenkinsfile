pipeline {
    agent any
    stage('build Success'){

         env.NODE_ENV = "test"

         echo "will succeed"
         print "Environment will be : ${env.NODE_ENV}"

         sh 'node -v'
         sh 'npm install'
         sh 'node app'
         sh 'mocha test/success.js'

       }

       stage('build Failure'){

         echo "will fail"

         sh 'node -v'
         sh 'npm install'
         sh 'node app'
         sh 'mocha test/error.js'

       }
}