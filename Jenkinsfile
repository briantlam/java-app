pipeline
{
	agent any
	tools
	{
		maven 'my-mvn'
	}

	stages
	{
		stage("Checkout")
		{
			steps
			{
				git url: 'https://github.com/briantlam/java-app.git'
			}
		}
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
