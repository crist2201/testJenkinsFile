pipeline {
	 agent any
	 stages {
		 stage("Go to directort"){
			 steps{
			 	bat 'cd qa-academy-at7-module4-api-automation-main'
			 }
		 }
		stage("buildOther") {
			 steps {
				 bat 'gradle clean build'
			 }
		}
		 stage("testOther") {
			 steps {
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
