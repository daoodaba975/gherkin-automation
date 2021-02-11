# Gherkin

## YouTube

FEATURE Publier une nouvelle vidéo  

SCENARIO Publication réussi  
GIVEN j’ouvre mon navigateur connecter sur la page web de YouTube  
THEN je vérifie la page web de YouTube en inspectant l’url  
WHEN j’appuie sur le bouton "Connexion"  
AND j'entre <mon-adresse-email> dans le champ email  
AND j'appuie sur le bouton "Continuer"  
AND j’entre <mon-mot-de-passe> dans le champ du mot de passe  
AND j'appuie sur le bouton "Connexion"  
THEN je vérifie si je suis sur mon compte YouTube  
WHEN j'appuie sur le bouton "Créer"  
AND j'appuie sur le bouton "Mettre en ligne une vidéo"  
AND je sélectionne <la-video>  
AND j'appuie sur le bouton "Publier"  
THEN la vidéo a été publié  

SCENARIO Echec publication : erreur connexion  
GIVEN j’ouvre mon navigateur connecter sur la page web de YouTube  
THEN je vérifie la page web de YouTube en inspectant l’url  
WHEN j’appuie sur le bouton "Connexion"  
AND j'entre <mon-adresse-email> dans le champ email  
AND j'appuie sur le bouton "Continuer"  
THEN la connexion est impossible  
