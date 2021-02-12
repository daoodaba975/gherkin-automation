# Gherkin

## Jumia

FEATURE Commander sur Jumia  

SCENARIO Commande réussi  
GIVEN j’ouvre mon navigateur connecter sur la page web de Jumia  
THEN je vérifie la page web de Jumia en inspectant l’url  
WHEN j’appuie sur le bouton "Se Connecter"  
AND j'entre <mon-adresse-email> dans le champ email  
AND j’entre <mon-mot-de-passe> dans le champ du mot de passe  
AND j'appuie sur le bouton "Connexion"  
THEN je vérifie si je suis sur mon compte Jumia  
WHEN je sélectionne <une-article> à commander  
THEN je vérifie si je suis sur la page de l'article  
WHEN j'appuie sur le bouton "Commander"  
AND j'entre <mes-coordonnes>  
AND j'appuie sur le bouton "Payer"  
THEN la commande est validé  

SCENARIO Echec commande : erreur connexion  
GIVEN j’ouvre mon navigateur connecter sur la page web de Jumia  
THEN je vérifie la page web de Jumia en inspectant l’url  
WHEN j’appuie sur le bouton "Se Connecter"  
AND j'entre <mon-adresse-email> dans le champ email  
AND j’entre <mon-mot-de-passe> dans le champ du mot de passe  
AND j'appuie sur le bouton "Connexion"  
THEN je vois un message d'erreur indiquant échec de connexion  

SCENARIO Echec commande : erreur paiement  
GIVEN j’ouvre mon navigateur connecter sur la page web de Jumia  
THEN je vérifie la page web de Jumia en inspectant l’url  
WHEN j’appuie sur le bouton "Se Connecter"  
AND j'entre <mon-adresse-email> dans le champ email  
AND j’entre <mon-mot-de-passe> dans le champ du mot de passe  
AND j'appuie sur le bouton "Connexion"  
THEN je vérifie si je suis sur mon compte Jumia  
WHEN je sélectionne <une-article> à commander  
THEN je vérifie si je suis sur la page de l'article  
WHEN j'appuie sur le bouton "Commander"  
AND j'entre <mes-coordonnes>  
AND j'appuie sur le bouton "Payer"  
THEN je vois un message d'erreur indiquant solde de insuffisant pour effectuer le paiement  
