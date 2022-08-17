pipeline {
    agent any
    stages {
        stage('Read CSV file content') {
            steps {
                script {
                    def file = new File('C:/Users/hmilahay/Desktop/jenkins_jobs.csv')
                    def map = file.collect{it}
                    map.each { 
                        stage (it) {
                                build "$it"
                        }
                    }
                }
            }
        }
    }
}
