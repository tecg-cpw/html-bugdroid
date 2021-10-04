# "Bugdroid"

> CSS exercise given at HEPL

* * *

**"Bugdroid"** is an educational project, which will be used for `HTML`/`CSS` courses.

**Note:** the school where the course is given, the [HEPL](http://www.provincedeliege.be/hauteecole) from Liège, Belgium, is a french-speaking school. From this point, the instruction will be in french. Sorry.

* * *

> Lors de vos cours de *web*, vous allez découvrir les langages HTML et CSS et les mettre en pratique pour apprendre à créer des pages web.  

* * *

## BugDroid

Vous trouverez dans ce dossier un fichier texte nommé **index.txt**. Cette page présente le robot Bugdroid.  

Votre mission est

1. de créer le fichier HTML qui permet d’afficher ce contenu dans un navigateur web&nbsp;;
2. de valider votre code HTML dans un validateur&nbsp;; 
3. de compléter (avec l’aide de votre professeur de labo) la feuille de style qui donnera à cette page le rendu suivant&nbsp;:

![rendu final](./rendu.png)

### 1. Création du fichier HTML

Pour vous aider, voici les étapes que vous pouvez suivre&nbsp;:

1. avant tout, et avant de commencer à taper du code dans un fichier, prenez le temps d’analyser le contenu fourni pour identifier les balises à utiliser. Vous pouvez vous aider du rendu ci-dessus pour identifier les grandes sections de la page. Si vous hésitez, vous pouvez également consulter l’aide fournie dans la section **«&nbsp;Aides&nbsp;»** ci-dessous&nbsp;;

2. créer le fichier HTML et y placer les balises de départ qui fournissent un template de base complet, ce qui implique notamment de bien indiquer que le document est en français et aussi&nbsp;:
	- au niveau de l'en-tête du document, de bien définir les méta-informations grâce aux balises `meta`, `title`et `link` appropriées (si vous avez besoin d’aide, voir la section **«&nbsp;Ressources&nbsp;»** ci-dessous) pour&nbsp;: 
	    * déclarer correctement l’encodage des caractères utilisé (pour ne pas avoir de problème d’affichage des caractères spéciaux et accentués dans le navigateur)&nbsp;;
	    * renseigner que vous êtes l’auteur du document&nbsp;;
	    * prévoir que, si on recherche votre page sur un moteur de recherche comme Google, les mots-clés suivants soient associés&nbsp;: BugDroid, mascotte Android, robot vert&nbsp;;
	    * prévoir que, si on recherche votre page sur un moteur de recherche comme Google, le moteur de recherche affiche la description suivante pour votre page dans la page qui présente les résultats de recherche&nbsp;: «&nbsp;Faites la connaissance de Bugdroid, le petit robot vert qui sert de mascotte à Android&nbsp;»&nbsp;
	    * faire en sorte que le titre du document qui s’affiche dans l’onglet du navigateur soit «&nbsp;BugDroid&nbsp;»&nbsp;;
	    * lier la feuille de style à votre page HTML&nbsp;;
	    * ~~prévoir que, si votre page est affichée dans un ancien navigateur IE qui ne reconnaît pas les nouvelles balises HTML5 (comme `nav`, `section`, etc.), ces dernières puissent malgré tout être correctement affichées par le navigateur en question (voir la section **«&nbsp;Ressources&nbsp;»** ci-dessous)~~(obsolète, plus nécessaire)&nbsp;;
	- au niveau du coprs du document, de découper la page en trois grandes sections :
	 	 * la bannière (balise `header`)&nbsp;;
	 	 * le contenu principal (balise `main`)&nbsp;;
	 	 * le pied ed page (balise `footer`)&nbsp;;
    
3. baliser le texte en utilisant les balises HTML correctes&nbsp;;

4. afficher l’image représentée dans le fichier `bugSkate.png` avec, comme texte alternatif au cas où elle ne s’affiche pas, «&nbsp;BugDroid, un petit robot vert, sautant sur son skate board&nbsp;»&nbsp;;

5. faire en sorte que le lien «&nbsp;Je découvre&nbsp;» mène vers le site officiel de BugDroid à l’adresse http://www.bugdroid.fr.

### 2. Validation du code HTML

1. lancer un validateur&nbsp;:
    - soit **HTML Validator** (extension de Firefox) *offline*&nbsp;;
    - soit le [validateur HTML5 du W3C](https://validator.w3.org/#validate_by_upload) *online*&nbsp;;
2. interpréter les erreurs éventuelles fournies par le validateur&nbsp;;
3. corriger&nbsp;;
4. valider à nouveau jusqu'à ce qu’il n’y ait plus d'erreur.  

### 3. Aides

#### 3. 1. Liste des balises

Étant donné que ceci est votre premier exercice en solo et que vous n’avez pas encore vu en cours théorique toutes les balises requises, voici la liste des balises HTML dont vous aurez besoin pour réaliser cet exercice : `html` (avec l'attribut `lang`), `head`, `meta` (avec les attributs `charset`, `name`, `content`), `title`, `link` (avec les attributs `rel` et `href`), `body`, `header`, `h1`, `i` (avec l'attribut `lang`), `main`, `p`, `dfn` (avec l'attribut `lang`), `abbr` (avec les attributs `lang` et `title`), `figure`, `img` (avec les attributs `src`, `alt`, `width`, `height`), `figcaption`, `b`, `a` (avec les attributs `href`, `title`, `hreflang`), `footer`, `time` (avec l'attribut `datetime`).

#### 3. 2. Rappel concernant les commentaires en HTML

- les commentaires en HTML s'indiquent entre les symboles `<!--` (marqueur de début de commentaire) et `-->` (marqueur de fin de commentaire). Tout ce qui se trouve entre ces deux marqueurs est ignoré par le navigateur, ce sont des textes qui ne sont ni affichés dans la page, ni interprétés par le navigateur. Ils sont réservés à l’usage exclusif du développeur. Vous pouvez y indiquer tout ce qui vous aide à comprendre, à organiser ou à relire votre code. Voici un exemple :

```html
    <!-- balise meta pour l'encodage des caractères --> 
    <meta charset="utf-8"> <!--  déclare au navigateur que l'encodage des caractères du document courant
                                 est réalisé en UTF-8 --> 
```

- ~~les commentaires conditionnels s’indiquent entre les symboles `<!--[if lt IE …]` (marqueur de début de commentaire conditionnel) et `<![endif]-->` (marqueur de fin de commentaire conditionnel). Tout ce qui se trouve entre ces deux marqueurs est ignoré par les navigateurs récents et n’est lu QUE par les navigateurs qui respectent la condition. Par exemple, ce qui se trouve dans le commentaire suivant (entre `<!--[if lt IE 9]>` et `<![endif]-->`) n’est exécuté QUE par les navigateurs IE antérieurs à IE9 :~~ (obsolète, plus nécessaire)

```html
<!--[if lt IE 8]>
    <link rel="stylesheet" href="css/screen-ie678.css">
<![endif]-->
```

#### 3. 3. Astuce pour démarrer beaucoup plus vite

Si vous utilisez Sublime Text et que l’extension *Emmet* est installée, il existe un raccourci clavier qui vous permet d’obtenir beaucoup plus rapidement un *template* de base qu’il vous suffira de compléter / modifier en fonction de vos besoins.

Presser simplement les touches `!` et `TAB` de votre clavier. Cela vous donnera déjà le résultat suivant&nbsp;: 

```html
<!DOCTYPE html>
<html lang="fr">
    <head>
        <meta charset="utf-8">
        <meta name="description" content="Description">
        <title>Document</title>
    </head>
    <body>
        
    </body>
</html>
```

Il vous suffit de changer la langue du document (de `en` en `fr`), de remplacer le mot-clé « Description » dans l’attribut `content` par votre vraie description et d’ajouter les balises manquantes.


### Ressources

> Ces ressources sont à consulter impérativement, elles font partie de la matière de cours

- [Référence des éléments HTML](https://developer.mozilla.org/fr/docs/Web/HTML/Element) : Une documentation qui reprend la liste des balises et leur sens, facile, en français issue du *MDN Web Docs* de Mozilla, une excellente référence&nbsp;;
- [HTML Living Standard](https://html.spec.whatwg.org/multipage/text-level-semantics.html#the-abbr-element) : **LA** spécification officielle du w3c/whatwg pour le langage HTML, c’est elle qui détient la vérité et qui fait loi en cas de doute. Il s’agit d’une documentation plus technique, en anglais, très complète, qui comporte une page par balise où on trouve toutes les informations nécessaires (sens, règles de grammaire, attributs, …). Votre «&nbsp;*Précis et Concis*&nbsp;» est une version imprimée de ce site&nbsp;; 
- [Comment indiquer la langue d’un contenu en HTML&nbsp;?](https://www.alsacreations.com/astuce/lire/1151-langue-du-contenu.html) : Aidez-vous de cette ressource pour savoir où et comment utiliser l’attribut lang dans les différents cas de figure&nbsp;;
- [ISO 639-1 Language Codes](https://www.w3schools.com/tags/ref_language_codes.asp) : Aidez-vous de cette ressource pour trouver quel est le code de langue à utiliser pour remplir correctement la valeur de l'attribut lang&nbsp;;
- [Un &lt;time&gt; pour chaque chose...](https://www.alsacreations.com/article/lire/1386-html5-element-time.html) : Aidez-vous de cette ressource pour trouver quel est le format de date à utiliser pour remplir correctement la valeur de l'attribut datetime dans la balise time&nbsp;;
- [À quoi servent les balises META ?](https://www.alsacreations.com/article/lire/628-balises-meta.html) : Aidez-vous de cette ressource pour correctement baliser les méta-informations à indiquer dans l’en-tête de votre document&nbsp;; 
- ~~[The HTML5 Shiv](https://github.com/afarkas/html5shiv). Aidez-vous de cette ressource pour télécharger les fichiers nécessaires et installer HTML5 Shiv, qui permet aux anciens navigateurs d’utiliser les nouvelles balises HTML5. N.B. Utilisez la procédure d’installation manuelle~~(obsolète, plus nécessaire).

* * *

Code par [Myriam Dupont](https://github.com/myriamdupont) d’après un code de Vincent de Oliveira.
