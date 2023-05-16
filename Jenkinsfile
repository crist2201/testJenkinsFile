pipeline {
	 agent any
	 stages {
		stage("buildOther") {
			 steps {
				 bat 'cd qa-academy-at7-module4-api-automation-main'
				 bat 'gradle clean build'
			 }
		}
		 stage("testOther") {
			 steps {
				 bat 'cd qa-academy-at7-module4-api-automation-main'
				 bat 'gradle clean executeFeature -D environmentName="QA" -DcucumberTags="@regression"'
			 }
		 }
		 stage("deployOther") {
			 steps {
				 bat 'echo new deply'
			 }
		 }
	 }
 }
