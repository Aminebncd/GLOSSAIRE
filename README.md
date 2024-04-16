
# GLOSSAIRE

- [Général](#général)
- [Front-end](#front-end)
- [UX / UI](#ux-ui)
- [Programmation orientée objet (POO)](#POO)
- [Architecture](#architecture)
- [Modélisation / Base de données](#modélisation---base-de-données)
- [Symfony](#symfony)
- [Sécurité](#sécurité)
- [RGPD](#rgpd)
- [SEO](#seo)
- [Gestion de projets / DevOps](#gestion-de-projets---devops)
- [English](#english)


## Général

1.	Quel est l’environnement à installer pour exécuter un script PHP ? Citer 2 exemples de logiciels permettant ce contexte  
      Réponse : pour exécuter un script PHP, chez ELAN nous utilisons LARAGON mais d’autres environnements comme XAMPP, WampServer ou Vagrant.
  	
2.	Qu’est-ce qu’un algorithme ?  
      Réponse : un algorithme est une suite d’instructions ayant pour but d’obtenir un résultat bien précis à partir de données que l’on lui aura fourni au préalable.
  	
3.	Qu’est-ce qu’une variable ? Par quel symbole est préfixée une variable en PHP ?  
      Réponse : une variable (caractérisée par le symbole $ en PHP) est un espace associant un nom à une valeur dans lequel on pourra stocker une donnée dans le but d’y faire appel plus tard dans le code.
  	
4.	Qu’est-ce que la portée d’une variable ?  
      Réponse : en fonction de si elle est locale, globale ou superglobale elle aura une portée de, respectivement, la fonction dans laquelle elle est declarée, le fichier tout entier ou l’ensemble de fichiers dans lesquels on travaille.
  	
5.	Qu’est-ce qu’une constante ? Quelle est la différence avec une variable ?  
      Réponse : comme son nom l’indique, une constante est une donnée dont la valeur restera inchangée à laquelle on peut faire appel partout dans notre code
  	
6.	Qu’est-ce qu’une superglobale, combien en existent-ils et donner un exemple d’utilisation.  
      Réponse : une superglobale est une variable native (pas besoin de la déclarer) à l’environnement dans lequel on travaille à laquelle on peut faire appel à travers tous nos fichiers. Il en existe 9 en PHP, parmi elles existe par exemple la variable $_GET récupère les données transmises en URL (query string).
   	
7.	Quels sont les différents types (primitifs) que l’on peut associer à une variable en PHP ? Les citer et en donner des exemples (ne pas oublier le type d’une variable sans valeur).  
      Réponse : une variable peut-être de type string (chaine de caractère : ‘test1212’), int (chiffre : 12345), float (chiffre à virgule : 1.256654), bool (true/false), array (tableau[]) et null si rien ne lui est attribué.
   	
8.	Existe-t-il plusieurs types de tableaux en PHP, si oui lesquels ?  
      Réponse : Il en existe deux, les tableaux associatifs (key => value) et les tableaux indexés sans clé ( ‘val1’, ‘val2’, ‘val3’…).
   	
9.	Quelles sont les différentes structures de contrôles qu’il existe en algorithmie ? Donner un exemple pour chacune d’entre elles.  
      Réponse : Il existe deux types de structures de contrôle, les conditions (if/else switch) qui, comme leur nom l’indique, vérifient une condition avant d’exécuter des instructions (if ($a < 1) { $a++ ;}  par exemple) et les boucles (for, while, do-while, foreach) qui, tant qu’une condition est respectée, vont répéter des instructions jusqu’à ce qu’elle ne soit plus valide (for ($i = 0 ; $i<10 ; $i++) {echo $i ;} par exemple)
   	
10.	Quelle est la fonction PHP permettant de demander la longueur d’une chaîne de caractères ?  
      Réponse : c’est la fonction strlen() ;
   	
11.	Qu’est-ce qu’une session ? Quelle fonction permet de démarrer une session en PHP ? Donner un exemple d’utilisation en PHP.  
      Réponse : Une session permet de stocker des données entre plusieurs accès, chaque visiteur accédant à une page web se voit attribuer un id de session pouvant être stocké dans un cookie. La fonction qui permet de démarrer une session en PHP est : session_start()
   	
12.	Qu’est-ce qu’un cookie ? Donner un exemple d’utilisation en PHP.  
      Réponse : Un cookie est un petit fichier texte contenant une quantité limitée de données, ils sont stockés coté client et peuvent être supprimé quand ils le souhaitent. Ils contiennent généralement des données de session permettant de faciliter la vie des utilisateurs comme des identifiants par exemple.
   	 
13.	Quelle est la différence entre les instructions « require » et « include » en PHP.  
      Réponse : si le fichier est manquant, require rendra une erreur (E_COMPILE_ERROR) et stoppera le script, include ne rendra qu’un avertissement (E_WARNING) et exécutera quand même le script.
   	
14.	Comment effectuer une redirection en PHP?  
      Réponse : Avec la fonction header(); (par exemple header(‘Location : monScript.php’); )
   	
15.	Définir la partie « front-end » et « back-end » d’une application.   
      Réponse : le Front-end est toute la partie ‘client’ qui apparaitra à l’utilisateur, le texte, le style, les images, les interactions physiques etc... le Back-end est toute la partie ‘serveur’ qui se passe en coulisse et n’apparait pas sur l’ordinateur de l’utilisateur, les traitements, la base de donnée, etc...
   	
16.	Définir le contrôle de version ? Qu’est-ce que Git?  
      Réponse : Le contrôle de version (ou versionning en anglais) représente le suivi et la gestion des changements apportés à une application. Il se gère avec des outils de versionnage appelés CVS, le plus populaire aujourd’hui s’appelle GIT.
   	
17.	Qu’est-ce qu’un CMS ? Citer au moins 2 exemples.  
    Réponse : Un CMS (Content Management System) est un programme permettant la création de sites web, les plus rependus sont Wordpress, Shoppify, Webflow et plein d’autres.
   	

## Front-end

1. Définir HTML  
   Réponse : HTML signifie « HyperText Markup Language » qu'on peut traduire par « langage de balises pour l'hypertexte ». Il est utilisé afin de créer et de représenter le contenu d'une page web et sa structure.

2. Définir CSS  
   Réponse : CSS est l’acronyme de « Cascading Style Sheets » ce qui signifie « feuille de style en cascade ». Le CSS correspond à un langage informatique permettant de mettre en forme des pages web.

3. Définir Javascript  
   Réponse : Javascript est un langage de programmation qui permet de créer du contenu mis à jour de façon dynamique sur une page web, de contrôler le contenu multimédia, d'animer des images, et tout ce à quoi on peut penser.

4. Définir JSON. Dans quel contexte ce format est-il utilisé ?  
   Réponse : Le JavaScript Object Notation (JSON) est un format standard utilisé pour représenter des données structurées de façon semblable aux objets Javascript. Il est habituellement utilisé pour structurer et transmettre des données sur des sites web (par exemple, envoyer des données depuis un serveur vers un client afin de les afficher sur une page web ou vice versa).

5. Peut-on interpréter du Javascript côté serveur ? Si oui, comment ?  
   Réponse :  Il existe aujourd'hui plusieurs solutions qui permettent d'exécuter du JavaScript côté serveur :

   - NodeJS initialement lancé en 2013 est la solution la plus répandue à l'heure actuelle.
   - Deno est une tentative du créateur de NodeJS de repartir sur de nouvelles bases. Même si la technologie est intéressante, elle a du mal à obtenir suffisamment de traction (principalement à cause de son incompatibilité avec l'écosystème NodeJS déjà présent).
   - Bun est une initiative toute jeune (pas encore stable) qui se veut être une alternative à NodeJS en promettant notamment d'être compatible avec l'existant.

6. Qu’est-ce qu’un sélecteur CSS ?  
   Réponse : Sélecteur CSS définit l’élément sur lequel s’applique le style voulu (type, identifiant, classe...).

7. Quelle balise HTML permet de créer un lien hypertexte ?  
   Réponse : C’est la balise anchor (<a href=”monLien”></a>).

8. Qu’est-ce qu’une requête AJAX ?  
   Réponse : L'ajax est une technique de développement web qui permet d'actualiser une partie d'une page sans la recharger entièrement. On évite ainsi le clignotement désagréable, les interactions avec l'utilisateur sont plus fluides.

9. Quel sélecteur CSS permet de sélectionner tous les éléments d’une classe spécifique ? D’un identifiant spécifique ?  
   Réponse : pour une classe “.maClasse”, pour un id “#monId”.

10. Définir le responsive design  
    Réponse : un design dit “responsive” s’adapte automatiquement aux changements de taille d’écran.

11. Qu’est-ce que le templating ?  
    Réponse : c’est pré-créer un modèle, un moule dans lequel on intégrera toutes nos pages web afin de ne pas avoir à re définir sur chaque page les éléments redondants (head etc…).

12. Qu’est-ce qu’une fonction anonyme en Javascript ?  
    Réponse : Une fonction anonyme n’a, comme son nom l’indique, pas de nom.

13. Quelle méthode JavaScript est utilisée pour ajouter un élément à la fin d'un tableau ?  
    Réponse : c’est Array push().

14. Qu’est-ce qu’un « media query » ?  
    Réponse : Elles permettent de modifier l’apparence d’un site ou d’une application en fonction du type d’appareil et de ses caractéristiques (la taille d'écran par exemple).

15. Qu’est-ce qu’un pseudo-élément en CSS ?  
    Réponse : c’est un mot-clé ajouté à un sélecteur qui permet de mettre en forme certaines parties de l’élément ciblé par la règle.

16. Qu’est-ce que Bootstrap ? Donner d’autres exemples équivalents  
    Réponse : c’est un framework de front-end gratuit qui permet de mettre en un site/une application plus « facilement », l’alternative la plus connue s’appelle Tailwind.

17. Quand un formulaire HTML est créé, quelles sont les 2 méthodes qui peuvent lui être associées ? Donner la différence entre ces 2 méthodes  
    Réponse : On peut utiliser la méthode POST (les données seront envoyées dans le corps de la requête HTTP) et GET (les données seront envoyées à travers l’URL).


## UX UI

1.	Quelle est la différence entre UX Design et UI Design ?  
      Réponse : L’UX c’est gérer l’experience utilisateur, la rendre intuitive, compatible avec tous les supports et facile d’utilisation. L’UI c’est travailler l’interface, l’information transmise, la clarté et la visibilité d’une application.
   	
2.	Qu’est-ce qu’un wireframe ?  
      Réponse : C’est une maquette très simpliste qui définit la structure d’un site
   	
3.	Qu’est-ce qu’un prototype ?  
      Réponse : C’est une maquette donnant un rendu quasi-fini du site/de l’application telle qu’on la veut.
   	 
4.	Qu’est-ce que la hiérarchie visuelle en UI Design ?  
      Réponse : La hiérarchie visuelle d'une page permet à l'utilisateur de savoir où concentrer son attention, son regard. Cette hiérarchie ordonne l'information, et permet de guider l'utilisateur lors de son parcours.
   	
5.	Qu’est-ce que l’accessibilité en UX Design ?  
      Réponse : L’accessibilité numérique, c’est rendre les produits numériques accessibles en situation de handicap.
   	
6.	Qu’est-ce qu’une grille de mise en page ?  
      Réponse : La grille est un élément déterminant de la mise en page, permettant de structurer le format.
   	
7.	Qu’est-ce que la notion d’affordance en UX Design ?  
      Réponse : L’affordance est la capacité d’un objet ou d’un système à évoquer son utilisation, sa fonction, elle permet de rendre l’utilisation d’un objet ou d’un service « intuitive ».
   	
8.	Qu’est-ce qu’un « mobile first design » ?  
      Réponse : C’est une stratégie de conception de réalisation de sites web en commençant par les versions mobiles afin d’optimiser au mieux le développement.

    
## Programmation orientée objet (POO)

1.	Donner une définition de la programmation orientée objet  
    Reponse : Approche de programmation basée sur la création de classes et d'objets qui interagissent entre eux pour réaliser des fonctionnalités. La POO vise à organiser le code de manière modulaire et à favoriser la réutilisabilité et la maintenance.
   	
2.	Qu’est-ce qu’une classe ? Comment la déclare-t-on ?  
      Reponse : Modèle ou plan de construction permettant de créer des objets. Elle est déclarée avec le mot-clé class suivi du nom de la classe.
   	
3.	Qu’est-ce qu’un objet ?  
      Reponse :  Instance concrète d'une classe. Un objet possède des attributs (propriétés) et des méthodes (fonctions) spécifiques à sa classe.
   	
4.	Définir la notion de propriété / attribut / méthode  
      Reponse : -Propriété -> Variable appartenant à un objet.  
                -Attribut ->  Synonyme de propriété, représente une caractéristique de l'objet.  
                -Méthode -> Fonction associée à une classe, permet de définir le comportement des objets de cette classe.  
   	
5.	Qu’est-ce que la visibilité d’une propriété ou d’une méthode ? Citer les différents types de visibilité  
      Reponse :  Contrôle l'accès aux propriétés et méthodes d'une classe. On peut la définir en temps que public, protected et private.
   	
6.	Quelle est la méthode spécifique utilisée pour créer un nouvel objet à partir d’une classe ?  
      Reponse :  Le constructeur, défini dans une classe avec la méthode __construct().
   	
7.	Qu’est-ce que l’encapsulation ?  
      Reponse :  Principe de la POO qui empêche de modifier ou d’accéder aux objets par un autre moyen que les méthodes proposées, et de ce fait, permet de garantir l’intégrité des objets.
   	
8.	Que signifie « étendre une classe » ? Quelle est le concept clé mis en œuvre ? Donner un exemple  
      Reponse : Permet à une classe enfant d'hériter des propriétés et méthodes d'une classe parente. Le concept clé est l'héritage. Exemple : class Voiture electrique extends Voiture.
   	
9.	Définir l’opérateur de résolution de portée  
      Reponse : Utilisé pour accéder aux éléments d'une classe. En PHP, l'opérateur est -> pour accéder à une propriété ou une méthode d'un objet.
   	
10.	Définir une méthode / propriété statique  
      Reponse :  Une méthode ou une propriété statique en programmation orientée objet est une entité qui appartient à la classe elle-même plutôt qu'à une instance spécifique de cette classe. Cela signifie que ces méthodes et propriétés sont partagées entre toutes les instances de la classe et peuvent être appelées sans avoir besoin d'instancier la classe.
   	
11.	Définir le polymorphisme en POO  
      Reponse : Le polymorphisme en programmation orientée objet fait référence à la capacité d'un objet à se comporter de différentes manières en fonction du contexte dans lequel il est utilisé. Cela signifie qu'un même nom de méthode peut avoir des implémentations différentes selon la classe à laquelle appartient l'objet qui l'appelle.
   	
12.	Définir une méthode / classe abstraite ?  
      Reponse : Une méthode ou une classe abstraite en programmation orientée objet (POO) est une entité déclarée dans une classe parente mais qui n'est pas implémentée dans cette classe. Au lieu de cela, les classes filles sont responsables d'implémenter ces méthodes ou de définir les détails de la classe abstraite.
   	
13.	Définir le chaînage de méthodes  
      Reponse : Technique permettant d'appeler plusieurs méthodes successivement sur le même objet en utilisant la même ligne de code. (par exemple $this->getUser()->getId() )
   	
14.	Qu’est-ce que la méthode __toString() ? Existe-t-il d’autres méthodes « magiques »  
      Reponse :  La méthode __toString() est une méthode spéciale en PHP qui est automatiquement appelée lorsqu'un objet est utilisé dans un contexte de chaîne de caractères, tel que lorsqu'il est passé à la fonction echo ou lorsqu'il est concaténé avec une chaîne de caractères.
   	
15.	Qu’est-ce qu’un « autoload » ?  
      Reponse : L'autoload est un mécanisme en PHP permettant de charger automatiquement les classes lorsqu'elles sont utilisées pour la première fois dans un script PHP. Au lieu de charger manuellement chaque classe avec la fonction require ou include chaque fois qu'elles sont nécessaires, l'autoload détecte automatiquement quand une classe est utilisée et charge son fichier correspondant, generalement avec la fonction 'spl_autoload_register()'.
   	
16.	Comment appelle-t-on en français les « getters » et les « setters » ?  
      Reponse :  En français, on les appelle respectivement "accesseurs" et "mutateurs". Ce sont des méthodes permettant de récupérer et de modifier les valeurs des propriétés privées d'une classe.
   	
17.	Qu’est-ce que la sérialisation en PHP ?  
      Reponse : La sérialisation en PHP est un processus qui consiste à convertir des objets PHP en une forme pouvant être stockée ou transmise, généralement dans le but de persister des données ou de les échanger avec d'autres systèmes. La sérialisation permet de transformer des données complexes, telles que des objets ou des tableaux, en une séquence de caractères qui peut être écrite dans un fichier ou envoyée sur un réseau.
   	

## Architecture 

1.	Qu’est-ce que l’architecture client / serveur ? Grâce à quel type de requête peut-on interroger le serveur. Définir l’acronyme de ce type de requête. Si on ajoute un « S » à cet acronyme, expliquer la différence  
      Reponse : L'architecture client/serveur est un modèle où les tâches sont partagées entre des ordinateurs appelés clients et des ordinateurs appelés serveurs. Les clients envoient des demandes aux serveurs, qui répondent en conséquence.

Pour interroger le serveur, on utilise souvent des requêtes HTTP. HTTPS est une version sécurisée de HTTP, qui chiffre les données pour une communication plus sécurisée.

2.	Donner la définition d’un design pattern. Citer au moins 3 exemples de design pattern  
      Reponse : Un design pattern est une solution éprouvée à un problème de conception logicielle courant. Voici trois exemples :

Singleton : Garantit qu'une classe a une seule instance.
Factory Method : Définit une interface pour créer des objets, laissant aux sous-classes le choix des classes concrètes à instancier.
Observer : Établit une relation un-à-plusieurs entre objets, permettant à certains objets d'être notifiés automatiquement des changements survenus dans d'autres objets.

3.	Qu’est-ce que l’architecture MVC ?  
      Reponse : L'architecture MVC divise une application en trois parties principales :

Modèle : Gère les données et les règles métier.
Vue : Affiche l'interface utilisateur.
Contrôleur : Traite les demandes des utilisateurs et coordonne les interactions entre le modèle et la vue.

4.	Quel est le rôle de chaque couche du design pattern MVC : Model, View, Controller ?  
      Reponse : Dans le design pattern MVC :

Modèle (Model) : Il représente les données de l'application ainsi que les règles métier qui s'appliquent à ces données. Le modèle gère la logique sous-jacente de l'application, y compris la manipulation des données, la validation et la logique métier.

Vue (View) : Elle est responsable de l'affichage des données au utilisateur. La vue récupère les données du modèle et les présente de manière appropriée à l'utilisateur. Elle ne manipule pas les données, mais se concentre uniquement sur leur affichage.

Contrôleur (Controller) : Il agit comme un intermédiaire entre la vue et le modèle. Il reçoit les demandes de l'utilisateur, traite ces demandes en interagissant avec le modèle approprié et met à jour la vue en conséquence. Le contrôleur gère également la logique de routage, déterminant quelle action doit être effectuée en fonction des demandes de l'utilisateur.

5.	Quels sont les avantages de l’architecture MVC ?   
      Reponse : Les avantages de l'architecture MVC sont la séparation claire des responsabilités, la modularité du code, la facilité de maintenance, la réutilisabilité du code, l'évolutivité de l'application et la facilitation de la collaboration entre développeurs.

6.	Existe-t-il des variantes à l’architecture MVC ?  
      Reponse : Oui, il existe des variantes à l'architecture MVC, telles que MVVM (Model-View-ViewModel), MVP (Model-View-Presenter), et MMVC (Multicore Model-View-Controller). Chacune de ces variantes adapte le modèle de base de MVC pour répondre à des besoins spécifiques ou des contextes particuliers de développement logiciel.

7.	Qu’est-ce qu’une API ? Définir l’architecture REST  
      Reponse : Une API (Interface de Programmation d'Application) permet à différents logiciels de communiquer entre eux. L'architecture REST (Representational State Transfer) est un style d'architecture qui utilise HTTP pour accéder et manipuler des ressources sur le web, en suivant des principes comme l'utilisation de ressources identifiées par des URI et l'utilisation d'opérations standard comme GET, POST, PUT et DELETE.

## Modélisation - Base de données

67.	Qu’est-ce que la modélisation de données ? Définir la méthode Merise

68.	Quelles sont les 3 étapes principales de la méthode Merise ? 
a.	Analyse, conception et réalisation
b.	Planification, exécution et contrôle
c.	Création, modification et suppression

69.	Qu’est-ce qu’un modèle conceptuel de données (MCD) en Merise ?

70.	Qu’est-ce qu’un modèle logique de données (MLD) en Merise ?

71.	Donner la définition des mots suivants :
a.	Entité
b.	Relation
c.	Cardinalité
d.	Clé primaire / clé étrangère

72.	Que devient une relation de type « Many To Many » dans le modèle logique de données ?

73.	Qu’est-ce qu’une base de données ?

74.	Définir les notions suivantes : 
a.	SQL
b.	MySQL
c.	SGBD (donner 2 exemples de SGBD)

75.	Dans une base de données, les données sont stockées dans des ___. Celles-ci sont constituées de lignes appelées ___ et de colonnes appelées ___

76.	Quelle est la différence entre une base de données relationnelle et non relationnelle ?

77.	Qu’est-ce qu’une jointure dans une base de données ? En existe-t-il plusieurs ? Si oui lesquelles ?

78.	A quoi sert une vue dans une base de données ?

79.	Qu’est-ce que l’intégrité référentielle dans une base de données ?

80.	Quelles sont les fonctions d’agrégation en SQL ?

81.	Qu’est-ce qu’un CRUD dans le contexte d’une base de données ?

82.	Quelles sont les clauses qui permettent de :
a.	Insérer un nouvel enregistrement dans une table
b.	Modifier un enregistrement dans une table
c.	Supprimer un enregistrement dans une table
d.	Supprimer la base de données
e.	Filtrer les résultats d’une requête SQL
f.	Trier les résultats d’une requête SELECT
g.	Regrouper les résultats d'une requête SELECT en fonction d'une colonne spécifique
h.	Concaténer 2 chaînes de caractères 

83.	Comment se connecter à une base de données en PHP ? Quelle est la classe native utilisée ?

## Symfony
84.	Qu’est-ce que Symfony ?
85.	Sur quel langage de programmation et design pattern repose Symfony ? 
86.	Quelle est la dernière version en date de Symfony ?
87.	Qu’est-ce qu’un bundle ? 
88.	Quel est le moteur de template utilisé par défaut dans Symfony ?
89.	Qu’est-ce qu’un ORM ? Quel est son utilité et comment s’appelle-t-il au sein de Symfony ?
90.	Qu’est-ce que l’injection de dépendances ? Quel est l’outil utilisé dans ce contexte et quel fichier contient l’intégralité des dépendances du projet ?
91.	Que permet le bundle Maker au sein de Symfony ? 
92.	Quel est le langage de requêtage exploité au sein d’un projet Symfony ?
93.	Quel est le composant qui garantit l’authentification et l’autorisation des utilisateurs ?

## Sécurité
94.	Qu’est-ce que l’injection SQL ? Comment s’en prémunir ?
95.	Qu’est-ce que la faille XSS ? Comment s’en prémunir ?
96.	Qu’est-ce que la faille CSRF ? Comment s’en prémunir ?
97.	Définir l’attaque par force brute et l’attaque par dictionnaire
98.	Existe-t-il d’autres failles de sécurité ? Citer celles-ci et expliquer simplement leur comportement
99.	A quoi servent l’authentification et l’autorisation dans un contexte d’application web ?
100.	Définir la notion de hachage d’un mot de passe et citer des algorithmes de hachage
101.	Qu’est-ce qu’une politique de mots de passe forts ?
102.	Qu’est-ce que l’hameçonnage ?
103.	Définir la « validation des entrées »

## RGPD
104.	Qu’est-ce que le RGPD ?
105.	Quel est son objectif principal ?
106.	Quelle est la date d’entrée en vigueur du RGPD ?
107.	Quelles sont les sanctions possibles en cas de non-respect du RGPD ?
108.	En France, quel est l’autorité administrative qui s’occupe de faire appliquer le RGPD ?
109.	Quel est le consentement valide selon le RPGD ?
110.	Qu’est-ce qu’une politique de confidentialité ?
111.	Quelle est la durée de conservation maximale des données personnelles selon le RGPD ?
112.	Quels sont les droits des utilisateurs selon le RGPD ?
113.	Qu’est-ce que le principe de minimisation des données selon le RGPD ?

## SEO
114.	Qu’est-ce que le SEO ? 
115.	Quel est l’objectif principal du SEO ?
116.	Existe-t-il plusieurs types de référencement ? Lesquels ?
117.	Qu’est-ce que la densité de mots-clés en SEO ?
118.	Qu’est-ce qu’une balise « alt » ?
119.	Qu’est-ce que la balise « meta description » ?
120.	Qu’est-ce que le « nofollow » en SEO ?
121.	Quelle est l'importance du contenu de qualité pour le référencement d'un site web ?
122.	Pourquoi est-il important d'utiliser des balises de titre (h1, h2, h3, etc.) de manière structurée ?
123.	Quelle est la recommandation pour les URL d'un site web bien référencé ?
124.	Qu'est-ce que le maillage interne et pourquoi est-il important pour le référencement ?
125.	Qu'est-ce que l'optimisation des images pour le référencement ?
126.	Qu'est-ce qu'un plan de site (sitemap) et pourquoi est-il important pour le référencement ?

## Gestion de projets - DevOps
127.	Qu’est-ce que la gestion de projet ?	
128.	Qu’est-ce qu’une méthode Agile de gestion de projet ? 
129.	Expliquer la méthode MoSCoW en quelques lignes et citer ses avantages
130.	A quoi sert la méthodologie MVP ? Citer les caractéristiques clés
131.	Qu’est-ce que la planification itérative ?
132.	Citer 3 méthodes Agiles dans le cadre d’un projet informatique
133.	Qu’est-ce qu’une réunion de revue de projet ?
134.	Qu’est-ce qu’un livrable dans un projet ? 
135.	Quels sont les 3 piliers SCRUM ? Définir chacun d’entre eux
136.	Qu’est-ce que le DevOps et quel est son objectif principal ?
137.	Qu’est-ce que l’intégration continue ? 
138.	Qu’est-ce que Docker ? Et en quoi est-il utile dans le cadre du DevOps ?
139.	Qu’est-ce qu’un test unitaire ? 
140.	Quelle est l'unité de code testée lors d'un test unitaire ?
141.	Quelles sont les caractéristiques d'un bon test unitaire ?
142.	Qu'est-ce qu'une assertion dans un test unitaire ?
 
## English
1)	What does JavaScript enable you to do on a website ?
a.	Add interactive behavior and dynamic content
b.	Define the layout and design of web pages
c.	Handle server-side operations
2)	Which programming language is primarily used for server-side web development ?
a.	PHP
b.	JavaScript
c.	HTML
3)	What is the purpose of a web browser ?
a.	To render and display web pages
b.	To execute serve-side code
c.	To manage databases
4)	What is the difference between GET and POST methods in HTTP ?
a.	GET retrieves data from a server, while POST submits data to a server
b.	GET submits data to a server, while POST retrieves data from a server
c.	GET and POST methods are interchangeable
5)	What is the purpose of version control systems (e.g., Git) in web development ?
a.	To track changes and manage collaborative development
b.	To optimize website loading speed
c.	To handle server-side scripting
6)	What is the purpose of a framework in web development ?
a.	To provide a structured environment for building web applications
b.	To handle network protocols and data transfer
c.	To create visual designs and layouts for websites
7)	What does NoSQL stand for ?
a.	Not Only SQL
b.	Non-Structured Query Language
c.	New Object-Oriented Language
8)	Which of the following is a characteristic of NoSQL databases ?
a.	Strict schema enforcement
b.	Support for complex transactions
c.	Scalability and flexible data models
