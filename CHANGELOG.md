# Notes de version

Chaque version publiée a sa section ici : l'outil de publication refuse une version qui n'en
a pas, et c'est ce texte qui accompagne la version sur GitHub.

## 1.0.2

- **Règles :** plus de case « par chantier ». Un SI qui parle du chantier
  (`{{projet.motsCles}}`…) cherche lui-même le chantier, où qu'il soit dans la règle : une
  règle s'écrit comme on la pense — « pas d'étiquette → si c'est un chantier, sa réception ;
  sinon si CR… ; sinon triage manuel ». Écrite ainsi, elle échouait sans la case, et avec elle
  ne cherchait que le premier chantier de la liste. Les règles existantes continuent de marcher.
- **Règles :** la complétion propose `{{projet…}}` dans les SI, et les dossiers du chantier sous
  un SI qui l'a trouvé. L'enregistrement prévient quand un `{{projet…}}` est placé là où aucun
  chantier n'aura été trouvé.
- **Correction :** annuler une exécution de règle rend aussi les étiquettes. Quand la règle
  avait étiqueté puis rangé un message, l'annulation le remettait bien dans son dossier mais lui
  laissait ses étiquettes.
- **Apparence :** le logo DEXO de la barre de gauche est bleu en thème sombre, noir en thème
  clair. En thème sombre, Thunderbird 156 affichait le logo sombre, à peine visible.

## 1.0.1

- **Correction :** le chat n'affiche plus le mot « null » au-dessus de tes messages quand ils
  n'ont pas de fichier joint.

## 1.0.0

Mise aux normes pour la publication sur la boutique des modules de Thunderbird
(addons.thunderbird.net). Aucun changement de fonctionnement : DEXO passe en version 1.0.0.

## 0.1.19

- **Longueur de contexte à 32K par défaut**, au lieu de 16K : de quoi lire un compte rendu de
  plusieurs pages et tenir une longue conversation. À baisser dans les réglages avancés si ta
  carte graphique a peu de mémoire vidéo. Un réglage déjà enregistré n'est pas modifié.

## 0.1.18

Première version publique.

- **Chat** intégré à Thunderbird : chercher, résumer, étiqueter, ranger, préparer des
  réponses. DEXO ouvre la fenêtre de rédaction, il n'envoie jamais rien.
- **Règles de tri** : conditions, bibliothèque de chantiers reconnus sur des mots entiers,
  étapes qui font appel au modèle (classer, résumer, extraire), simulation avant activation,
  annulation d'une exécution.
- **Pièces jointes** : lecture des PDF, Word, Excel et des scans ; résumé dans le chat, par
  clic droit ou dans une règle ; fichiers joints directement au chat.
- **Profil** : ton nom et ton entreprise, pour que DEXO repère ce qui te concerne.
- **Mises à jour** : Thunderbird installe les nouvelles versions depuis GitHub ; DEXO signale
  quand le programme local doit être mis à jour.
