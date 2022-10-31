@startuml
left to right direction 
skinparam packageStyle rectangle
skinparam actorStyle awesome
actor "Visiteur" as v
actor "Administrateur" as a
actor "Utilisateur" as u

v <|-- u
u <|-- a

rectangle OpenObservatory {
  useCase "Créer un compte" as UC1
  useCase "Consulter les observations" as UC2
  useCase "Regarder les profils utilisateurs" as UC3
  useCase "Poster des observations" as UC4
  useCase "Voter sur des observations" as UC5
  useCase "Modifier son profil" as UC6
  useCase "Modifier ses paramètres de notification" as UC7
  useCase "Se déconnecter" as UC8
  useCase "Administrer les objets célestes" as UC9
  useCase "Administrer les observations" as UC10
  useCase "Gestion des utilisateurs" as UC11
  UC11 .> (Supprimer un utilisateur) : include
  UC11 .> (Ajouter/Retirer des privilèges à un utilisateur) : include
  UC2 .> (Afficher une carte) : extend
  UC2 .> (Localiser la station ISS) : include 
  UC4 .> (Modifier ses observations) : include
}

actor "API externe" as api1
actor "API externe" as api2
api1 -> (Localiser la station ISS)
api2 -> (Afficher une carte)
v -> UC1
v -> UC2
v -> UC3
u -> UC4
u -> UC5
u -> UC6
u -> UC7
u -> UC8
a -> UC8
a -> UC9
a -> UC10
a -> UC11

@enduml