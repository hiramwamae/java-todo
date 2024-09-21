pipeline{
    agent any
    tools{
        gradle 'gradle'
    }
        stages{
            stage('cloning code'){
                steps{
                    git branch: 'master', url: 'https://github.com/hiramwamae/java-todo'
                }
            }
            stage('Building Code'){
                steps{
                    sh 'gradle build'
                }
            }
            stage('Testing Code'){
                steps{
                    sh 'gradle test'
                }
            }
        }

}