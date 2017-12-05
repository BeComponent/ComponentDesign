# Dialogue

Idée d'appli : site de certification de projet _Useless_ sur Github
Fonctionnalités : 
  - Liste des projets
  - Liste des profils
  - Profil et ses projets
  - Projets et ses contributeurs
  - Formulaire de soumission de projet
  
Dialogue :
  
- J'ai fait une appli pour répertorier un projet inutile (donc un dispensable) qui s'appellerait __Best of Useless__.
  Problème : 
    - 2 composants listes => 1 composant générique qui prend en entrée un composant item de liste (projet, profil)
    - Ajouter le détail d'un projet dans le formulaire => l'afficher dans les cartes projet
- Cool
- Par contre dès que je veux modifier ça il faut que je modifie à ces 10 autres endroit pour impacter tout l'appli
- On va regarder ce que t'as fait
- <Gros composant bien blindé>
- 😱 C'est normal, ce truc devrais être une brique communique partagée par tout le monde. Je vais te montrer comment tu peux redécouper ton appli

Timeline:
 - 5 gros templates (1 par vue) + controller => __duplication de code__ => [Atomic] Découpage en composants génériques
 - Port de la donnée par les composants => __pas réutilisabilité__ => [Container/Presentational]
 - Passage de la donnée dans l'arbre de composants => __centralisation de la donnée__ => [Store]
 
