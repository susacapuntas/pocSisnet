pipeline {
    agent none
	parameters {
		choice(
			name: 'selectjob',
			choices: "PoC_Sisnet_MdP\nPoC_Sisnet_DAS",
			description: "Job build selection")
	}
    stages {
		stage('PoC_SISnet'){
			steps {
				build job:"${params.selectjob}"
			}
        }
    }
}