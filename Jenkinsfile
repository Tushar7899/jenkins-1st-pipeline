pipeline {
    agent {
        node {
            label 'lable1'
            customWorkspace '/home/ubuntu/a/workspace'
        }

    }
    stages {
        stage('git commit') {
            steps {
                git 'https://github.com/swapnibrad/studentapp-ui.git'
            }
        }
        stage('build') {
            steps {
                sh '''
                mkdir github_dir
                echo "successfully copied file"
                '''
            }
        }
        stage('test') {
            steps {
                echo "successfully test"
            }
        }
        stage('deploy') {
            steps {
              echo "successfully deployed"
            }
        }
        stage('run script') {
            steps {
            script {
                def name = "cloudblitz"
                def gender = "male"
                if(gender == "male") {
                    echo "Mr. $name"    
                } else {
                    echo "Mrs. $name"
                }
            }
        }
        }
    }
}
