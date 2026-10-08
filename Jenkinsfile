pipeline{
   agent any
   stages{
     stage('Fetching the code from remote repo'){
         steps {
          git branch: 'main', url: 'https://github.com/dhanunjayasneha/maven.git'
           }
       }
     stage('build phase'){
        steps{
          build 'maven'
        }
      }
     stage('testing phase'){
          steps{
             echo 'this is a testing stage'
         }
       }
     stage('deploy phase'){
         steps{
            echo 'deploy information'
          }
       }
    }
 }

