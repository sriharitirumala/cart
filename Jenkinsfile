@Library('roboshop') _


    pipeline {
        agent any

        stages {

            stage('Compile/Build') {
                steps {
                    script {
                        common.compile()
                    }
                }
            }

            stages {

                stage('Unit Test Cases') {
                    steps {
                        script {
                            common.unittestcases()
                        }
                    }
                }
            }
        }
    }


env.component = "cart"
env.app_lang  = "nodejs"
env.notify_group = "sritirumala30@gmail.com"

ci()