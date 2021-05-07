Skip to content
Search or jump to…

Pull requests
Issues
Marketplace
Explore
 
@athakkar9033 
devopscube
/
declarative-pipeline-examples
1
7
23
Code
Issues
Pull requests
Actions
Projects
Wiki
Security
Insights
declarative-pipeline-examples/parameters/Jenkinsfile.staticParametes
@devopscube
devopscube Create Jenkinsfile.staticParametes
Latest commit 92c249f on Aug 12, 2020
 History
 1 contributor
36 lines (36 sloc)  1.22 KB
  
pipeline {
    agent any
    stages {
        stage('Setup parameters') {
            steps {
                script { 
                    properties([
                        parameters([
                            choice(
                                choices: ['ONE', 'TWO'], 
                                name: 'PARAMETER_01'
                            ),
                            booleanParam(
                                defaultValue: true, 
                                description: '', 
                                name: 'BOOLEAN'
                            ),
                            text(
                                defaultValue: '''
                                this is a multi-line 
                                string parameter example
                                ''', 
                                 name: 'MULTI-LINE-STRING'
                            ),
                            string(
                                defaultValue: 'scriptcrunch', 
                                name: 'STRING-PARAMETER', 
                                trim: true
                            )
                        ])
                    ])
                }
            }
        }
    }   
}

