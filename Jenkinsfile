pipeline {
	 agent any
	 stages {
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
