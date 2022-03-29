# AtelierBackEnd

Le BackEnd seras seulement autoriser pour les admins de l'application.

Les admins ont donc une interface d'authentification qui leur permette de se connecter se la gestion des utilisateurs.

Ils peuvent donc supprimer des utilisateurs, se rediriger sur une route pour afficher les utilisateurs inactifs...


La création d'un compte admin s'éffectue avec PostMan nous devons inscrire le liens suivanrt : http://149.91.80.75:19380/register

Nous utilisons Body -> raw pour pouvoir insérer dans une moustache l'email et le mot de passe :
{
    "email":"admin2@mail.fr",
    "password":"admin"
}

On utilse POST et nous faisons un send. Le mot de passe seras crypté et nous aurons la génération d'un Token qui s'afficheras dans la base de donnée.
