# comue.watcha.fr — ComUE / Université de Lyon

Gabarits propres à l'instance dont le `server_name` est `comue.watcha.fr`.
Le déploiement Synapse (`devops/prod/deploy-synapse-from-host.sh`) copie `fr/`
puis ce dossier par-dessus : un fichier présent ici remplace son homologue de `fr/`.

- `watcha_registration.html` / `.txt` : mail d'invitation validé par le client —
  « Un utilisateur de l'Université de Lyon », connexion recommandée par Renater ou
  ProConnect, **aucun mot de passe affiché** (« Mot de passe oublié » à la
  première connexion), puis lien de connexion depuis le navigateur (bouton
  Watcha + `login_url`).

Toute modification faite directement sur le serveur est écrasée au déploiement
suivant : modifier ici. Penser à répercuter ici une évolution du mail standard
(`fr/watcha_registration.*`) si elle doit aussi s'appliquer à ComUE.
