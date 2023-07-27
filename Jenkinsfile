pipeline {
    agent any 

     parameters {

    choiceParam('environment', ['QA'],
    'Which environment to apply testing to')

    choiceParam('browser', ['chrome'],
    'Browser to run tests on')

    choiceParam('config_file', ['CucumberConfig/nightwatch.conf.js'],
    'configuriation file to use for nightwatch')

    choiceParam('test_tag', ['logindetails','IITSmoke'],
    'Test Tag that applies to which test or suite of test to run')
    
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
