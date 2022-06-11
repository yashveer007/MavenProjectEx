pipeline{
	agent any
	parameters { 
		string(name: 'Tag', defaultValue: '', description: 'please pass the tag ')
		booleanParam(name: 'test', defaultValue: true, description: ' enable test cases')
	}
	stages{
		stage("Setup"){
			steps{
				echo "this is do setup ${params.Tag}"
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
