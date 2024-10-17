pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh 'python -m py_compile sources/add2vals.py sources/calc.py sources/test.py' 
                stash(name: 'compiled-results', includes: 'sources/*.py*') 
            }
        }
    }
}
