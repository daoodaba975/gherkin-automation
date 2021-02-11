# Gherkin

## Facebook

FEATURE Partager un post sur Facebook  

SCENARIO Partage réussi  
GIVEN j’ouvre mon navigateur connecter sur la page web de Facebook  
THEN je vérifie la page web de Facebook en inspectant l’url  
WHEN j’entre <mon-adresse-email> dans le champ email  
AND j’entre <mon-mot-de-passe> dans le champ du mot de passe  
AND j'appuie sur le bouton "Connexion"  
THEN je vérifie si je suis sur mon compte Facebook  
WHEN j'appuie sur le champ "Que voulez vous dire"  
AND j'entre <mon-publication>  
AND j'appuie sur le bouton "Publier"  
THEN le post a été partagé  

SCENARIO Echec partage : erreur connexion  
GIVEN j’ouvre mon navigateur connecter sur la page web de Facebook  
THEN je vérifie la page web de Facebook en inspectant l’url  
WHEN j’entre <mon-adresse-email> dans le champ email  
AND j’entre <mon-mot-de-passe> dans le champ du mot de passe  
AND j'appuie sur le bouton "Connexion"  
THEN la connexion est impossible  

SCENARIO Echec partage : erreur contenu à partager  
GIVEN j’ouvre mon navigateur connecter sur la page web de Facebook  
THEN je vérifie la page web de Facebook en inspectant l’url  
WHEN j’entre <mon-adresse-email> dans le champ email  
AND j’entre <mon-mot-de-passe> dans le champ du mot de passe  
AND j'appuie sur le bouton "Connexion"  
THEN je vérifie si je suis sur mon compte Facebook  
WHEN j'appuie sur le champ "Que voulez vous dire"  
AND j'entre <mon-publication>  
AND j'appuie sur le bouton "Publier"  
THEN erreur sur le partage, à cause du dépassement du nombre caractére  
