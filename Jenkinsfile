pipeline{
	agent any
	parameters { 
		string(name: 'tag', defaultValue: '', description: 'please pass the tag ')
		booleanParam(name: 'test', defaultValue: true, description: ' enable test cases')
	}
	environment { 
        	github_org = "yashveer007"
		github_repo = "MavenProjectEx"
    	}
	stages{
		stage("Setup"){
			steps{
				echo "this is do setup ${params.tag}"
				echo "$github_org"
			}
		}
		stage("versioning"){
			steps{
				echo "this is do versioning ${params.tag} "
			}
		}
		stage("test"){
			steps{
				echo "this is do test ${params.tag}"
			}
		}
		stage("package"){
			steps{
				echo "this is do package ${params.tag}"
			}
		}
	}
}
