```plantuml
left to right direction 

hide circle
hide attribute
hide method

package Rôles{
    class Utilisateur
    class Administrateur
}

package Entités{
    class Message
    class Groupe
    class Compagnie
}


Administrateur -|> Utilisateur 

Utilisateur"*" --o "*"Groupe
Message"*" --* Groupe 
Groupe"*" --* Compagnie
Utilisateur"*" -down-o Compagnie 
Message"*" --* "2" Utilisateur

Compagnie"1" --* Administrateur
Groupe --o Utilisateur

```