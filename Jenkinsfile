pipeline {
	 agent any
	 stages {
		stage("buildOther") {
			 steps {
				 dir (qa-academy-at7-module4-api-automation-main){
				 	bat 'gradle clean build'
				 }
			 }
		}
		 stage("testOther") {
			 steps {
				 dir (qa-academy-at7-module4-api-automation-main){
				 	bat 'gradle clean executeFeature -D environmentName="QA" -DcucumberTags="@regression"'
				 }
			 }
		 }
		 stage("deployOther") {
			 steps {
				 bat 'echo new deply'
			 }
		 }
	 }
 }
