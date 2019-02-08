# Sonarqube

* Télécharger Sonarqube à cette [adresse](https://www.sonarqube.org/downloads/)
* Dézipper le fichier à l'endroit souhaité

Lancement du serveur Sonarqube :

* Avec un terminal, aller dans le dossier de Sonarqube
`cd <chemin_vers_le_dossier>`
* Avec Windows :
	- bin\windows-x86-xx\StartSonar.bat
* Avec un autre OS
	- bin/[OS]/sonar.sh start
* Accès à [SonarQube](http://localhost:9000)

Pour analyser un fichier `Java` :

*  Le projet doit être un projet Maven
*  Ajouter au pom.xml

```{xml}
<dependency>
    <groupId>org.codehaus.sonar</groupId>
    <artifactId>sonar-maven-plugin</artifactId>
    <version>5.1</version>
</dependency>
```
* Lancer la configuration Maven suivante

`clean install sonar:sonar`

PS : il faut penser à installer le `package` Maven à la première utilisation 
