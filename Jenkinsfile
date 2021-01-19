pipeline{
    agent any
    parameters{
        choice(name: 'choice', choices: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
        
    }
    stages{
         stage('init'){
            steps {
                script {
                    gv = load 'multiply.groovy'
                }
                echo 'Init application'
            }
         }
        stage('build') {
            steps {
                echo 'Building application'
            }
        }
        stage('test'){
            steps {
                echo 'Testing application'
            }
        }
        stage('deploy'){
            steps{
                echo 'Deploying application'
            }
        }
    }
}