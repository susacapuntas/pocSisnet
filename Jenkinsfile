pipeline {
    agent { label 'patata' }
    stages {
        stage('Test'){
			steps {
				try {
					build job:'PoC_Sisnet'
				} catch (Exception e) {
					println 'Existen test con errores'
				}
			}  
        }
    }
}