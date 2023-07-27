pipeline {
    agent any 

    parameters { choice(name: 'ENV', choices: ['Dev', 'QA', 'Prod'], description: 'enter the value') 
                 choice(name: 'browser', choices: ['browser'], description: 'browser value')
        }
    
    stages{
        stage("build"){
            steps {
                sh 'echo $ENV'
                
            }
        }
          stage("test"){
            steps {
                sh 'echo $browser'
            }
        }
    
}
}
