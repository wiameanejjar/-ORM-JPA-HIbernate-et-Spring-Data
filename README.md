# Rapport de TP – Application de Gestion Hospitalière avec Spring Boot et JPA

## 📌 Objectif du TP

L’objectif de ce TP est de développer une application de gestion hospitalière en utilisant le framework Spring Boot et Spring Data JPA.
Cette application permet de modéliser les principales entités d’un système hospitalier, telles que les patients, les médecins, les rendez-vous, les consultations, et leur gestion au travers de services et d’un contrôleur REST.

L'application doit permettre de :
 - Gérer les entités : Patient, Medecin, RendezVous, Consultation, et StatusRDV.
 - Ajouter, consulter et modifier les données associées à ces entités.
 - Organiser les services métiers liés aux opérations de gestion hospitalière.
 - Exposer une API REST pour interagir avec le système.
 - Utiliser une base de données embarquée (H2) pour stocker les données pendant l’exécution.

---

## 🧱 Structure du Projet

Le projet suit une architecture en couches typique d’une application Spring Boot :
 - entities : contient les classes de domaine représentant les entités métier :
    - Patient, Medecin, RendezVous, Consultation, StatusRDV.
 - repositories : contient les interfaces JPA permettant l’accès aux données :
    - PatientRepository, MedecinRepository, RendezVousRepository, ConsultationRepository.
 - service : contient l’interface métier IHospitalService et son implémentation HospitalServiceImpl, qui encapsulent la logique métier.
 - web : contient les contrôleurs REST exposant les endpoints de l’application : PatientRestController.
 - HospitalApplication : classe principale avec l’annotation @SpringBootApplication qui sert de point d’entrée à l’application.


  
