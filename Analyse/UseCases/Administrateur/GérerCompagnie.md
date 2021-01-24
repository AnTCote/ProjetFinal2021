# Cas d'utilisation - Gérer Compagnie

## Acteur(s) primaires et secondaires
Administrateur 

## Préconditions/déclencheur


## Postconditions


## Scénario de base : 
```plantuml
start
if () then (Creer)
    if (Admin possède 
    déjà compagnie?) then (non)
        :Entrer: 
        - Nom
        - Image ;
    else (oui)
        end
    endif
else(Modifier)
    :Modifier: 
    - Nom
    - Image ;

endif
stop 

```

## Exceptions
L'administrateur tente de créer une nouvelle compagnie alors qu'il en possède déjà une.
## Besoins non-fonctionnels spécifique