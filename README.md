# F-Tool

**Préparez votre montée en forgemagie et comparez les équipements selon votre budget.**

F-Tool est une application Windows dédiée aux joueurs de **DOFUS**. Elle compare le prix des runes à leur poids et propose des parcours d’équipements pour progresser dans les métiers de forgemagie, du niveau 1 au niveau 200.

Son interface rassemble les prix de votre serveur, les illustrations des objets et le budget des équipements à acheter.

![Accueil de F-Tool](<img width="2557" height="1357" alt="Capture d&#39;écran 2026-10-07 221534" src="https://github.com/user-attachments/assets/0e884afb-999d-450b-bc37-6a02dc67a910" />)

## Fonctionnalités

- **Runes Rentables** : classement des runes selon leur coût en kamas par point de poids.
- **Prix par serveur** : récupération des prix publics Huzounet et saisie manuelle, à l’unité ou par lot.
- **Parcours et budget** : proposition d’une progression avec les objets, leurs niveaux, les runes compatibles et le total des achats.
- **Rune commune** : sélection automatique ou choix d’une caractéristique à conserver au fil du parcours.
- **Comparaison des objets** : recherche par nom, filtre de niveaux et affichage des prix disponibles.
- **Prix manquants** : estimation indicative à partir des prix publics de trois autres serveurs.
- **Export CSV** : export de la comparaison ou du parcours pour consultation dans Excel.
- **Sauvegarde automatique** : conservation des prix et des préférences, avec des prix séparés pour chaque serveur.

## Les six métiers

| Métier | Équipements |
| --- | --- |
| Forgemage | Épées, dagues, marteaux, pelles, haches et lances |
| Sculptemage | Arcs, baguettes et bâtons |
| Costumage | Capes et chapeaux |
| Cordomage | Bottes et ceintures |
| Joaillomage | Anneaux et amulettes |
| Façomage | Boucliers |

## Installation

1. Téléchargez **F-Tool.exe** depuis la section **Releases** du dépôt.
2. Placez le fichier dans le dossier de votre choix.
3. Lancez l’application.

La version distribuée est un **exécutable autonome pour Windows 64 bits** : aucune installation séparée de .NET n’est nécessaire. Le catalogue et les images sont intégrés au fichier.

Une connexion Internet est nécessaire pour actualiser les prix. Les données déjà enregistrées, le catalogue et les illustrations restent disponibles hors connexion.

## Premiers pas

1. **Choisissez votre serveur** dans la liste en haut de la fenêtre.
2. Ouvrez **Runes Rentables** et cliquez sur **Actualiser les prix**.
3. Sélectionnez votre métier, puis actualisez les prix de ses équipements.
4. Dans **Parcours et budget**, indiquez votre niveau actuel, votre objectif et la rune commune souhaitée, ou laissez le mode **Automatique**.
5. Complétez les prix manquants en cliquant sur un encadré de prix, ou utilisez **Estimer les prix manquants**.
6. Consultez le budget et exportez votre parcours si nécessaire.

**Votre prix manuel reste toujours prioritaire sur le prix importé.** Vous pouvez revenir au prix automatique depuis la fenêtre de saisie.

## Un parcours adapté aux objets

F-Tool recherche des équipements dont les caractéristiques naturelles permettent d’utiliser les runes retenues. Il compare les prix disponibles pour proposer un enchaînement économique et conserver, autant que possible, une caractéristique commune.

Les changements suivent le **niveau réel des objets**, avec des étapes rapprochées au début et un écart maximal de **15 niveaux entre deux équipements**. La dernière pièce peut être conservée jusqu’au niveau 200 : un équipement de niveau 185 peut ainsi éviter un achat supplémentaire en fin de parcours.

![Exemple de parcours Cordomage](<img width="2555" height="1353" alt="Capture d&#39;écran 2026-10-07 221614" src="https://github.com/user-attachments/assets/83704f4c-bc43-4421-b8b8-b5898287b83b" />)

*Les captures présentent des données de démonstration. Les prix et les objets proposés varient selon le serveur, les prix renseignés et la rune choisie.*

### Règles de sélection des runes

Les runes de poids **inférieur à 3**, les runes sans poids et les familles **Fo, Ine, Cha et Age**, variantes Pa et Ra comprises, sont exclues du classement et de la sélection habituelle. Les runes de dommages élémentaires restent autorisées. Les runes de transcendance ne sont pas incluses.

Si ces règles empêchent de démarrer un métier, une exception temporaire autorise des runes exclues pour les premières étapes. Le parcours revient aux règles habituelles dès qu’un équipement compatible est accessible. Les runes sans poids restent toujours exclues.

### Comprendre le budget

Le budget correspond **uniquement au prix des équipements à acheter**, chaque objet étant compté une fois. Il n’inclut pas la consommation de runes.

Un prix inconnu reste à renseigner : il n’est jamais considéré comme gratuit. Le total devient alors un **sous-total à compléter**. Les prix estimés entre serveurs sont signalés par **≈** ; ils ne représentent pas une observation du marché de votre serveur.

Les propositions dépendent des prix disponibles et des familles de runes comparées. Elles ne garantissent donc pas le parcours le moins cher de tout le marché. L’XP affichée indique les seuils à atteindre ; l’application ne prédit pas le nombre de runes nécessaires ni les réussites de forgemagie.

## Données et illustrations

- **[DofusDB](https://dofusdb.fr/)** : catalogue des objets et des runes, caractéristiques, poids et pictogrammes des équipements, runes et métiers.
- **[Huzounet](https://huzounet.fr/market)** : prix publics par serveur et illustrations des serveurs.
- **Catalogue embarqué** : 2 834 équipements et 105 définitions de runes de forgemagie avant application des filtres, issus de l’import du 6 octobre 2026.

Le catalogue est un instantané embarqué. Les prix sont actualisés à votre demande, sans suivi permanent en arrière-plan.

## Retours et contributions

Vous pouvez signaler un problème ou proposer une amélioration dans les **Issues** du dépôt. Pour un parcours inattendu, précisez le métier, le serveur, les niveaux de départ et d’arrivée, la rune sélectionnée et les prix renseignés.

---

**Conception : Buddy.**
F-Tool est un projet indépendant, sans affiliation officielle avec Ankama, DofusDB ou Huzounet.
DOFUS et les éléments visuels du jeu appartiennent à leurs ayants droit.

