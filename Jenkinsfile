pipeline {  
 agent any  
 environment {  
  dotnet = 'C:\\Program Files\\dotnet\\dotnet.exe'  
 }  
 stages {  
  stage('Checkout') {  
   steps {  
    git credentialsId: 'b92a2c28-2693-4fc1-8490-49c7db00ed8a', url: 'https://github.com/sajidur/Donor.git', branch: 'master'  
   }  
  }  
 stage('Build') {  
   steps {  
    bat 'dotnet build Donor.sln --configuration Release'  
   }  
  }  
  stage('Test') {  
   steps {  
    bat 'dotnet build Donor.sln --configuration Release'  
   }  
  }  
 }  
}  
