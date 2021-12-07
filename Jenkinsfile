pipeline{
   agent any
	stages{
    	   stage('Build'){
             steps{
               bat 'dotnet build'
             }
        }   
        stage('archive'){
           archiveArtifacts(artifacts: '**/*.dll', followSymlinks: false)
        }
   }
}