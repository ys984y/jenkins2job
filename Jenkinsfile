pipeline {
    agent any 

     parameters {

    choice('environment', ['QA'],
    'Which environment to apply testing to')

    choice('browser', ['chrome'],
    'Browser to run tests on')

    choice('config_file', ['CucumberConfig/nightwatch.conf.js'],
    'configuriation file to use for nightwatch')

    choice('test_tag', ['logindetails','IITSmoke'],
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
