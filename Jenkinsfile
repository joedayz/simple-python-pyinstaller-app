pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                bat 'python3 --version'    
                bat 'python3 -m py_compile sources/add2vals.py sources/calc.py' 
                stash(name: 'compiled-results', includes: 'sources/*.py*') 
            }
        }


    }
}
