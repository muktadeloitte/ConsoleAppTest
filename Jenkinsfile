pipeline{
   agent any
	stages{
    	   stage('Build'){
             steps{
               bat 'dotnet build'
             }
        }   
        stage('archive'){
           steps{
              archiveArtifacts(artifacts: '**/*.dll', followSymlinks: false)
           }
        }
   }
}