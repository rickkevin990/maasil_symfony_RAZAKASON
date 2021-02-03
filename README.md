# maasil_symfony_RAZAKASON
PRE-REQUIS:
- version min => PHP 7.1.9 
- Mysql     
- Visual code ou IDE php 

0)configurer la base de donnee en modifiant le fichier ".env"
  DATABASE_URL="mysql://root:@127.0.0.1:3306/blog_maasil?serverVersion=5.7"
 => changer "root" par votre propre utilisateur  et ajouter votre mot de passe si il y en a , ou si non laisse le par DEFAUT

1)Creez une base de donnee en tapant juste dans la console :
  php bin/console doctrine:database:create


2) pour commencer, vous devez faire une migration en executant la commande suivante:
php bin/console make:migration

3) Puis pour l'executer dans votre base de donnee  il faut tapez la commande suivante:
php bin/console doctrine:migrations:migrate

4) ajouter quelque  donnee a l'aide d'un fixture (optionnel):
php bin/console doctrine:fixtures:load

l'utilisateur : Razakason
Mot de passe : kevin

5)Pour lancer l'application tapez sur dans la terminal le commande suivant:
-php bin/console server:run => permet de lancer le server 




BONUS:
lancer la commande pour faire un test du controller create article:
php bin/phpunit 
