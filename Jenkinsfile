pipeline {
    agent any 

    parameters { choice(name: 'ENV', choices: ['Dev', 'QA', 'Prod'], description: 'enter the value') 
                 choice(name: 'browser', choice: ['browser'], description: 'browser value')
        }
    
    stages{
        stage("build"){
            steps {
                sh 'echo $environment'
                
            }
        }
          stage("test"){
            steps {
                sh 'echo $browser'
            }
        }
    
}
}
