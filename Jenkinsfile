@Library('my-shared-library') _

pipeline {

    agent any
       
    stages{

        stage ('git checkout'){

            steps{

              gitCheckout(
                branch: "main",
                url: "https://github.com/vikash-kumar01/mrdevops_java_app.git"
            )  
            }
        }
        stage ('unit test maven'){

            steps{

             script{

                mvnTest()
             } 
            }
        }
    }   
}