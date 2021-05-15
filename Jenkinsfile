pipeline
{
	agent any
	tools
	{
		maven 'my-mvn'
	}

	stages
	{
		stage("Build")
		{
			steps
			{
				sh "mvn compile"
			}
		}
		stage("Unit Test")
		{
			steps
			{
				sh "mvn test"
			}
		}
	}
}
