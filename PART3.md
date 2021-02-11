# Gherkin

## GitHub

FEATURE Créer un repository  

SCENARIO Création repository réussi  
GIVEN j’ouvre mon navigateur connecter sur la page web de GitHub  
THEN je vérifie la page web de GitHub en inspectant l’url  
WHEN j’appuie sur le bouton "Connexion"  
AND j'entre <mon-adresse-email> dans le champ email  
AND j’entre <mon-mot-de-passe> dans le champ du mot de passe  
AND j'appuie sur le bouton "Connexion"  
THEN je vérifie si je suis sur mon compte GitHub  
WHEN j'appuie sur le bouton "New"  
AND j'appuie sur le bouton "New repository"  
AND j'appuie sur le bouton "Publier"  
AND j'entre le <nom-du-repository>  
AND j'appuie sur le bouton "Create"  
THEN le repository a été créé  

SCENARIO Echec création repository : erreur connexion  
GIVEN j’ouvre mon navigateur connecter sur la page web de GitHub  
THEN je vérifie la page web de GitHub en inspectant l’url  
WHEN j’appuie sur le bouton "Connexion"  
AND j'entre <mon-adresse-email> dans le champ email  
AND j’entre <mon-mot-de-passe> dans le champ du mot de passe  
AND j'appuie sur le bouton "Connexion"  
THEN la connexion est impossible  
