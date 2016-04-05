# UTBM Learning project

Projet d'étude dans le cadre de mon cursus à l'UTBM
Application de prise de rendez-vous pour un cabinet medical. 


## Architecture

Client / serveur -> 4 Modules  :

* rdvmedecins-api-core				(DAO & Business Layer / Spring Data JPA Hibernate , Spring Securité)
* rdvmedecins-api-ws				(Service Layer / REST web service with Spring MVC)
* rdvmedecins-api-web-springmvc		(web layer / Spring MVC & thymeleaf & jquery)
* rdvmedecins-api-web-jsf			(web layer / JSF 2 et primeface): JSF Page => ManagedBean => Service => DAO
	
* rdvmedecins-api-web-angularjs		(ui web / AngularJS 1)
(projet angular à part , généré avec yeoman, importer dans un projet maven web)
	
## Stack Technique

Côté serveur, on utilise les technologies

* [Spring Data] pour l'accès à la base de données;
* [Spring MVC] pour les services web;
* [JUnit] pour les TU
* [Spring Security] pour la sécurisation de celui-ci;
* [Mysql] - Pour le SGBD

Coté client

* [Angular ou JSF] - pour le front


# Outils utilisés

* Plateform : JDK 1.8
* IDE : Eclipse Mars (+ Spring Tools Suite)
* Application Server : Tomcat 7
* SCM : Git
* Build : Maven 3
* SGBD : WampServer (MySQL 5) - Workbench

# Features

l'utilisateur se connecte et 
peut ensuite choisir le médecin avec lequel on veut un rendez-vous et le jour de celui-ci 
voir l'agenda du médecin choisi pour le jour choisi ;
une fois obtenu l'agenda du médecin, on peut réserver un créneau
Une fois le rendez-vous validé, on est ramené automatiquement à l'agenda où le nouveau rendez-vous est désormais inscrit. Ce
rendez-vous pourra être ultérieurement supprimé

i18n  : FR & EN

	