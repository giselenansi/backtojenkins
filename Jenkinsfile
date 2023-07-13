pipeline {
    agent any
    
    stages {
        stage('Create User and Group') {
            steps {
                script {
                    sh '''
                        # Create a group
                        groupadd mygroup
                        
                        # Create a user
                        useradd -m myuser
                        
                        # Add the user to the group
                        usermod -a -G mygroup myuser
                    '''
                }
            }
        }
    }
}
