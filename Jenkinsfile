pipeline {
	 agent any
	 stages {
		stage("buildOther") {
			 steps {
				 bat 'qa-academy-at7-module4-api-automation-main/gradle clean build'
			 }
		}
		 stage("testOther") {
			 steps {
				 bat 'qa-academy-at7-module4-api-automation-main/gradle clean executeFeature -D environmentName="QA" -DcucumberTags="@regression"'
			 }
		 }
		 stage("deployOther") {
			 steps {
				 bat 'echo new deply'
			 }
		 }
	 }
 }
