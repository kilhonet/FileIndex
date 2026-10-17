# FileIndex

**Un outil de recherche de fichiers gratuit pour Windows qui trouve les fichiers de tout le PC dès que vous tapez un nom.**

[English](README.md) · [한국어](README.ko.md) · [简体中文](README.zh-CN.md) · [日本語](README.ja.md) · [Español](README.es.md) · [Português (Brasil)](README.pt-BR.md) · Français

> Ce document est une traduction. En cas de différence, la [version coréenne](README.ko.md) fait foi.

![Platform](https://img.shields.io/badge/platform-Windows%2010%20%2F%2011%20(64--bit)-0078D4)
![License](https://img.shields.io/badge/license-Freeware-brightgreen)
[![Download](https://img.shields.io/badge/download-kilho.net-orange)](https://down.kilho.net/fileindex?lang=fr)

![Écran de FileIndex](images/fileindex-en.png)

## Présentation

FileIndex recherche par nom de fichier sur tous les lecteurs du PC à la fois. Les résultats changent pendant que vous tapez dans la zone de recherche, et les noms coréens se trouvent même en ne tapant que leurs consonnes initiales (`ㅅㅈ` → 설정).

Au premier lancement, il dresse la liste des fichiers de chaque lecteur ; ensuite, il suit en temps réel les fichiers créés, supprimés et renommés, de sorte que les résultats sont toujours à jour. Vous pouvez combiner des conditions d'extension, de taille, de caractères génériques et d'expressions régulières, et il trouve aussi les fichiers en double de même nom, de même taille ou de même contenu.

Les fichiers trouvés s'ouvrent, se copient, se glissent-déposent et s'utilisent avec le menu contextuel comme dans l'Explorateur de fichiers. Fermer la fenêtre laisse FileIndex dans la zone de notification, prêt à revenir aussitôt, et pendant qu'il est masqué il n'utilise presque pas de mémoire.

## Fonctionnalités

- **Recherche au fil de la frappe** — trouve les noms contenant tous les mots séparés par des espaces. Sans distinction de casse.
- **Recherche par consonnes initiales coréennes** — taper simplement `ㅅㅈ` trouve des noms comme « 설정 » et « 사진 ».
- **Conditions de recherche** — extension (`ext:`), taille (`size:`), caractères génériques (`*` `?`), expressions régulières (`regex:`).
- **Recherche de doublons** — même nom (`dupe:name`), même taille (`dupe:size`), contenu identique (`dupe:content`).
- **Mise à jour en temps réel** — les changements de fichiers apparaissent aussitôt dans les résultats. Ce qui a changé pendant que FileIndex était fermé est rattrapé au démarrage.
- **Indexation automatique des lecteurs USB** — les lecteurs nouvellement branchés sont indexés d'eux-mêmes et retirés des résultats quand on les débranche.
- **Comme dans l'Explorateur** — double-clic pour ouvrir, ouvrir l'emplacement, sélection multiple et copie, glisser vers l'Explorateur, menu contextuel de l'Explorateur.
- **Aperçu** — affiche à côté de la liste la miniature du fichier sélectionné (photos, vidéos, PDF, documents Office, etc.).
- **Tri et surlignage** — tri par nom, chemin, taille ou date de modification ; la partie du nom qui correspond est surlignée.
- **Dans la zone de notification** — fermer la fenêtre la masque dans la zone de notification, où il n'utilise presque pas de mémoire.
- **Reste sur votre PC** — la liste des fichiers est enregistrée uniquement sur votre propre PC.
- **22 langues, thèmes clair et sombre** — suit les réglages de Windows par défaut, ou choisissez vous-même.

## Téléchargement / installation

| Type | Lien |
|---|---|
| Programme d'installation | [Télécharger](https://down.kilho.net/fileindex?lang=fr) |
| Version portable (ZIP) | [Télécharger](https://down.kilho.net/fileindex?lang=fr&nosetup) |

Le programme d'installation lance FileIndex à la fin et active **Lancer au démarrage**, de sorte qu'il démarre dans la zone de notification à chaque ouverture de session Windows. Pour la version portable, décompressez le ZIP et lancez `FileIndex.exe`. Les deux versions ont les mêmes fonctionnalités.

Lire rapidement des lecteurs entiers nécessite les droits d'administrateur ; Windows affiche donc une demande de confirmation administrateur au lancement de FileIndex. Cliquez sur **Oui**.

## Utilisation

### Premiers pas

1. Lancez FileIndex. La première fois, pendant qu'il dresse la liste des fichiers de chaque lecteur, le centre de la fenêtre affiche la progression, par exemple **C : indexation 42%**. Une fois terminé, l'écran de recherche apparaît.
2. Tapez une partie d'un nom de fichier dans la zone de recherche. Les résultats s'affichent dans la liste au fil de la frappe, et le nombre trouvé apparaît en bas.
3. **Double-cliquez** sur le fichier voulu, ou sélectionnez-le avec les flèches et appuyez sur **Entrée**, pour l'ouvrir dans le programme associé. Appuyez sur **Ctrl+Entrée** pour ouvrir le dossier qui le contient.
4. Quand vous avez fini, cliquez sur le bouton de fermeture (X) ou appuyez sur **Échap**. FileIndex ne quitte pas : il se masque dans la zone de notification. Cliquez sur son icône pour le faire réapparaître aussitôt.

À partir du deuxième lancement, FileIndex reprend la liste déjà établie et ne rattrape que ce qui a changé pendant qu'il était fermé ; vous pouvez donc chercher immédiatement.

### Éléments de l'écran

| Élément | Rôle |
|---|---|
| Zone de recherche | Saisissez un nom de fichier, des consonnes initiales ou des conditions de recherche. Le bouton flèche à droite relance la recherche avec le texte actuel |
| Liste des résultats | **Nom** · **Chemin** · **Taille** · **Modifié le**. Cliquez sur un en-tête de colonne pour trier ; faites glisser une bordure pour redimensionner une colonne |
| Aperçu | En bas à droite de la liste. Miniature du fichier sélectionné (masqué pour les fichiers sans miniature) |
| Barre d'état | Nombre de résultats. S'il y en a plus que le maximum, elle affiche affichés / total, par ex. `200 / 14,092 éléments` |
| Bouton des paramètres | Dans la barre de titre, à gauche du bouton de réduction. Ouvre la fenêtre **Paramètres** |
| Icône de notification | Clic gauche pour ouvrir la fenêtre. Le menu du clic droit propose **FileIndex** · **Auteur** · **Quitter** |

### Cas d'usage

**Trouver des noms coréens par leurs consonnes initiales**
En tapant seulement des consonnes coréennes, vous trouvez les noms dont les initiales apparaissent dans cet ordre. `ㄱㅇㅅ` trouve des noms comme « 계약서 » et « 계약서_수정본 », dont les initiales contiennent ㄱ, ㅇ, ㅅ dans l'ordre. Même les noms longs se trouvent en quelques touches.

**Affiner avec plusieurs mots**
Séparez les mots par des espaces et seuls les noms qui les contiennent tous restent. `rapport 2026` trouve les fichiers dont le nom contient à la fois « rapport » et « 2026 ». L'ordre des mots n'a pas d'importance.

**Ne chercher que certains types de fichiers**
Écrivez les extensions après `ext:`, séparées par des **points-virgules (;)**. Les dossiers sont exclus ; seuls les fichiers apparaissent.
- `ext:pdf` — tous les fichiers PDF
- `ext:jpg;png;gif voyage` — les images dont le nom contient « voyage »

**Trouver les gros fichiers pour libérer de l'espace**
Utilisez `size:` pour une condition de taille. Les unités sont `b` `kb` `mb` `gb` `tb` ; sans unité, ce sont des octets.
- `size:>1gb` — fichiers de plus de 1 Go
- `size:1mb-5mb` — de 1 Mo à 5 Mo inclus (`1mb..5mb` fonctionne aussi)
- `ext:mp4 size:>500mb` — vidéos de plus de 500 Mo

Triez les résultats par l'en-tête **Taille** pour voir d'abord les plus gros fichiers.

**Décrire la forme d'un nom avec des caractères génériques**
`*` correspond à un nombre quelconque de caractères et `?` à exactement un. Avec des caractères génériques, **le nom entier** doit correspondre au motif.
- `*.txt` — fichiers d'extension txt
- `readme*` — noms commençant par readme
- `IMG_????.jpg` — images avec quatre caractères après IMG_

**Chercher plus précisément avec des expressions régulières**
Écrivez une expression régulière après `regex:`. Elle ne distingue pas la casse et peut correspondre n'importe où dans le nom. Utilisez `^` et `$` pour ancrer le début et la fin ; comme les espaces séparent les termes de recherche, écrivez une espace dans un motif sous la forme `\s`.
- `regex:^\d{8}` — noms commençant par huit chiffres (comme une date)
- `regex:(draft|final)` — noms contenant draft ou final

Si une condition est mal écrite, la barre d'état affiche un exemple de la forme correcte.

**Faire le ménage dans les doublons**
`dupe:` regroupe les fichiers identiques et les affiche groupe par groupe. Combiné à d'autres conditions, il ne compare qu'à l'intérieur de ces résultats.
- `dupe:name` — fichiers de même nom (sans distinction de casse)
- `dupe:size ext:jpg` — images de même taille
- `dupe:content ext:mp4` — vidéos au **contenu strictement identique**

`dupe:content` lit réellement les fichiers pour les comparer ; la barre d'état affiche donc la progression sous la forme **Comparaison du contenu — fichiers n/N, x/y MB**. Modifier le texte de recherche arrête la comparaison. Dans chaque groupe, sélectionnez tout sauf l'exemplaire à garder, puis clic droit → Supprimer.

**Retrouver un fichier tout juste téléchargé**
Le tri par défaut est **Modifié le**, du plus récent au plus ancien : il suffit de taper une partie du nom pour que le fichier téléchargé ou modifié le plus récemment soit en haut. Les fichiers nouvellement créés ou enregistrés apparaissent aussitôt dans les résultats.

**Trop de résultats / tout afficher**
Par défaut, la liste affiche jusqu'à **200** résultats. La recherche porte toujours sur tout, trie puis affiche depuis le haut : vous obtenez donc « les 200 plus récents » ou « les 200 plus gros ». `200 / 14,092 éléments` dans la barre d'état signifie que 200 résultats sur 14 092 sont affichés. Pour en voir davantage, augmentez **Paramètres → Résultats max.**

**Copier ou déplacer plusieurs fichiers ailleurs**
- Sélectionnez-en plusieurs par **Ctrl/Maj + clic** ou **Maj + flèches**, ou appuyez sur **Ctrl+A** pour sélectionner tous les résultats.
- Appuyez sur **Ctrl+C**, puis collez dans l'Explorateur de fichiers.
- Vous pouvez aussi **glisser les fichiers sélectionnés vers l'Explorateur ou le Bureau**. Comme dans l'Explorateur, ils sont déplacés sur le même lecteur et copiés vers un autre lecteur.

**Utiliser le menu contextuel de l'Explorateur**
Faites un clic droit sur un résultat pour obtenir le même menu que dans l'Explorateur (Ouvrir avec, Envoyer vers, compresser, Supprimer, Propriétés, etc.). Maintenez **Maj** pendant le clic droit pour afficher aussi les commandes étendues. Les programmes lancés depuis ce menu s'exécutent avec les droits d'utilisateur normaux, pas en administrateur.

**Voir photos et documents sans les ouvrir**
Avec **Aperçu** activé (par défaut), une miniature apparaît en bas à droite de la liste chaque fois que vous sélectionnez un fichier. C'est la même miniature que dans l'Explorateur : vidéos, PDF et documents Office sont prévisualisés en plus des photos. Parcourez-les avec les flèches.

**Chercher sur des clés USB et disques externes**
Branchez-en un : en quelques secondes il est indexé et apparaît dans les résultats. Débranché, ses résultats disparaissent ; rebranché, il est indexé à nouveau.

**Au clavier uniquement**
Le focus reste toujours dans la zone de recherche : il suffit de taper.

| Touche | Action |
|---|---|
| ↑ ↓ / Pg préc Pg suiv | Sélectionner des résultats (maintenez Maj pour une plage) |
| Entrée | Ouvrir dans le programme associé (le premier résultat si rien n'est sélectionné) |
| Ctrl+Entrée | Ouvrir l'emplacement du fichier dans l'Explorateur |
| Ctrl+A / Ctrl+C | Sélectionner tous les résultats / copier les fichiers sélectionnés |
| Échap | Effacer le texte de recherche ; s'il est déjà vide, masquer dans la zone de notification |

**Ouvrir une recherche depuis un raccourci ou un script**
Indiquez une recherche après `--search` (ou `-s`) et FileIndex s'ouvre sur ces résultats. Si FileIndex tourne déjà, c'est la fenêtre ouverte qui lance cette recherche.

```
FileIndex.exe --search "ext:pdf contrat"
FileIndex.exe -s "*.psd"
```

Ajoutez-le à la cible d'un raccourci sur le Bureau pour ouvrir une recherche fréquente en un clic.

**Le laisser tourner et s'en servir comme d'un raccourci clavier**
Avec **Lancer au démarrage** activé, FileIndex démarre sans fenêtre dans la zone de notification à l'ouverture de session. Cliquez sur son icône quand vous en avez besoin : il apparaît avec le curseur déjà dans la zone de recherche, il n'y a plus qu'à taper. Pour le quitter complètement, clic droit sur l'icône → **Quitter**.

## Configuration

Ouvrez **Paramètres** avec le bouton des paramètres de la barre de titre. Les changements sont enregistrés et appliqués immédiatement.

| Section | Option | Par défaut |
|---|---|---|
| Général | Tri par défaut (Par nom · Par chemin · Par taille · Par date) | Par date |
| Général | Thème (Système · Clair · Sombre) | Système |
| Général | Langue (Système + 22 langues) | Système |
| Général | Résultats max. | 200 |
| Général | Aperçu | Activé |
| Général | Lancer au démarrage | Activé avec le programme d'installation |
| À propos | Version · Auteur · Site web · Licence | — |

**[Rétablir]** remet les paramètres à leurs valeurs par défaut et désactive aussi Lancer au démarrage. La liste de fichiers déjà établie est conservée. Changer de langue fait passer l'écran dans cette langue tout de suite, sans redémarrer.

## Configuration requise

- Windows 10 · Windows 11 (64 bits)
- Lecteurs formatés en NTFS (le format par défaut de Windows — disques internes comme lecteurs USB)
- Droits d'administrateur (cliquez sur **Oui** à la confirmation au lancement)
- Internet sert uniquement à vérifier les nouvelles versions. La recherche fonctionne hors ligne.

## Mises à jour

FileIndex ne se met **pas** à jour tout seul. Au démarrage, il vérifie s'il existe une nouvelle version et affiche un avis ; cliquer sur **[Oui]** ouvre la page de téléchargement et ferme le programme. Les nouvelles versions sont publiées manuellement après des tests internes et annoncées sur la [page de FileIndex](https://kilho.net/fileindex). Consultez l'[avis sur la politique de mise à jour](https://en.kilho.net/archives/notice/2940).

## Licence

FileIndex est un **gratuiciel** (freeware). Utilisez-le gratuitement partout — au bureau, à la maison, dans les administrations ou à l'école — et redistribuez-le librement.

## Liens

- Site web : <https://kilho.net/fileindex>
- Forum : <https://kilho.top/forum/qna>
- X (Twitter) : <https://www.twitter.com/kilhonet>

© KILHO.NET
