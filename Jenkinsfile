node {
  //stage('SCM') {
  //  git 'https://github.com/ravirajt01/sonarDemo.git'
 // }
  stage('SonarQube analysis') {
    withSonarQubeEnv() {
      // requires SonarQube Scanner for Gradle 2.1+
      // It's important to add --info because of SONARJNKNS-281
      sh './gradlew --info sonarqube'
    }
  }
}