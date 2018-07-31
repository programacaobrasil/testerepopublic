# testerepopublic

# Url para validar repositório
https://jitpack.io/

# Documentação
- https://jitpack.io/docs/ANDROID/
- http://helpdev.com.br/2016/10/28/android-github-maven-jitpack-disponibilizando-uma-biblioteca-android-como-dependencia-utilizando-o-github-jitpack-publishing-of-android-libraries/

# Para criar

# Project Gradle
buildscript { 
  dependencies {
    classpath 'com.github.dcendents:android-maven-gradle-plugin:2.1' // Add this line
 
# App Gradle
apply plugin: 'com.android.library'
apply plugin: 'com.github.dcendents.android-maven'  
group='com.github.YourUsername'
 
 # Executar
 gradlew install
 
 # Dá commit no arquivo
 gradlew

# Para importar
# Project Gradle
allprojects {
  repositories {
    ...
    maven { url 'https://jitpack.io' }
  }
}
  
# App Gradle:
dependencies {
        implementation 'com.github.programacaobrasil:testerepopublic:1.2'
}
