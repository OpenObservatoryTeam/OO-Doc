@startuml
alt Modification durée de validité des observations
    Administrateur -> Système : Modifie la durée de validité des observations
    Système ->  Système : Enregistrement de la durée 
    Système -> Administrateur : Affichage validation de la modification
else
    alt Modification d'une observaation
        Administrateur -> Système : Demande de modification d'une observation
        Système -> Administrateur : Affiche le formulaire de modification d'une observation
        Administrateur -> Système : Envoie formulaire modification
        Système -> Système : Validation du formulaire
        alt Formulaire invalide
           Système -> Administrateur : Affichage des erreurs
        else Formulaire valide
           Système -> Système : Enregistrement des modifications
        alt Erreurs de sauvegarde
           Système -> Administrateur : Affichage des erreurs
        else Pas d'erreurs de sauvegarde
           Système -> Administrateur : Affiche une validation de modification 
        end
    end
    else Supprimer une observation
         Administrateur -> Système : Demande de supression d'une observation
         Système -> Système : Supression de l'objet célestre
         alt Erreurs de suppression 
             Système -> Administrateur : Affichage des erreurs 
         else Pas d'erreurs de suppresion
             Système -> Administrateur : Affichage validation de suppression de l'observation 
        end
    end
end
@enduml