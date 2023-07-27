pipeline {
    agent any 

    parameters { choice(name: 'ENV', choices: ['Dev', 'QA', 'Prod'], description: 'enter the value') }
    
    stages{
        stage("build"){
            steps {
                sh 'echo $ENV'
            }
        }
    }
}
