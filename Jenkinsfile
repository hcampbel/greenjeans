node
{
    // Checkout Source Code
  stage('Checkout Source') {
      git credentialsId: '424706f6-ec71-4afa-a7b9-34f6e7731d07', 
      url: 'https://github.com/hcampbel/greenjeans.git'
  }

  // Use CMake Plugin to build application
  stage('Build Application') {

      cmakeBuild buildDir: 'build', 
      buildType: 'RelWithDebInfo', 
      installation: 'InSearchPath'

  }
}