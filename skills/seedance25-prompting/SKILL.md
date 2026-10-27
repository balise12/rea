---
name: seedance25-prompting
description: Concevoir, structurer et améliorer des prompts vidéo pour la page Seedance 2.5 de hunyuanvideo.org. À utiliser pour transformer une idée ou une image de référence en prompt vidéo clair, cinématographique et testable.
---

# Skill — Prompting vidéo pour Seedance 2.5

## Objectif

Aider l’utilisateur à produire des prompts exploitables pour le générateur Seedance 2.5 présenté sur https://www.hunyuanvideo.org/fr/seedance25. La page décrit des workflows texte-vers-vidéo et image-vers-vidéo et met l’accent sur le mouvement, la continuité du sujet, la fluidité de caméra, la cohérence de l’éclairage et la stabilité du décor.

Ne pas présenter les capacités, limites, réglages ou conditions commerciales de cette interface comme vérifiés au-delà de ce que l’utilisateur voit dans l’application. Le site précise qu’il s’agit d’un site indépendant, pas du site officiel Tencent Hunyuan. Ne pas promettre un résultat parfait.

## Comportement

1. Comprendre l’intention : publicité, scène narrative, clip produit, portrait, animation, B-roll, paysage ou autre.
2. Identifier le mode :
   - **Texte vers vidéo** : décrire le plan complet.
   - **Image vers vidéo** : préserver le sujet, la composition et les caractéristiques importantes de l’image source ; décrire principalement ce qui doit bouger et comment la caméra se comporte.
3. Si des informations essentielles manquent, poser au maximum une question courte. Sinon, choisir des hypothèses raisonnables et les signaler brièvement.
4. Rédiger un prompt visuel concret, sans contradictions ni accumulation de synonymes.
5. Répondre dans la langue de l’utilisateur. Pour les termes visuels, un prompt anglais peut être proposé en seconde version si cela lui est utile, sans affirmer que l’anglais est obligatoire.
6. Séparer le prompt prêt à copier des notes et des variantes.
7. Ne jamais inventer des paramètres d’interface (durée, ratio, résolution, seed, negative prompt, audio, etc.). Si ces contrôles sont présents dans l’interface, conseiller de les régler séparément selon le besoin.

## Structure recommandée du prompt

Utiliser cette structure souple et ne conserver que les éléments pertinents :

1. **Sujet principal** — qui ou quoi apparaît, caractéristiques distinctives.
2. **Action et trajectoire** — mouvement observable, direction, rythme, début et fin.
3. **Lieu et arrière-plan** — environnement, profondeur, éléments fixes.
4. **Caméra** — type de plan, angle, mouvement (travelling, panoramique, caméra fixe, suivi), vitesse et stabilité.
5. **Lumière et palette** — source, direction, contraste, température, couleurs dominantes.
6. **Style et matière** — réalisme, animation, publicité premium, documentaire, pellicule, textures.
7. **Temporalité** — évolution claire de la scène ; une action principale et, si utile, une action secondaire.
8. **Contraintes de cohérence** — garder l’identité et les vêtements du sujet, la disposition du décor, la géométrie des objets et une lumière cohérente.
9. **Composition finale** — où se trouve le sujet à la fin et comment le plan se termine.

### Gabarit

« [Sujet et caractéristiques] [action précise, direction et rythme] dans [lieu et détails du décor]. [Type de plan, angle et mouvement de caméra]. [Lumière, ambiance et palette]. [Style visuel et détails de texture]. Le sujet conserve [caractéristiques à préserver] ; le décor et l’éclairage restent cohérents. Le plan se termine par [état final / composition]. »

## Règles de qualité

- Préférer les verbes visibles : « tourne lentement la tête vers la fenêtre » plutôt que « ressent la nostalgie ».
- Décrire le mouvement avec une direction et une vitesse : « avance de deux pas vers la caméra, puis s’arrête ».
- Limiter le plan à une action principale. Pour plusieurs événements, préciser leur ordre.
- Donner à la caméra un comportement compatible avec l’action. Éviter de demander simultanément un plan fixe et un travelling.
- Décrire séparément le mouvement du sujet, celui de la caméra et les mouvements du décor.
- Pour les produits, préserver forme, proportions, étiquette, couleur et position ; éviter les transformations involontaires.
- Pour les visages et personnages, préciser les traits, la coiffure, les vêtements et les accessoires à conserver.
- Pour une image source, ne pas réinventer ce qui est déjà visible. Demander seulement les changements voulus.
- Remplacer les adjectifs vagues (« incroyable », « épique », « beau ») par des indices visuels concrets.
- Utiliser les contraintes négatives avec parcimonie et de manière positive lorsque possible : « mains naturelles et anatomie cohérente » plutôt qu’une longue liste de défauts.
- Ne pas surcharger le prompt de styles contradictoires, de mouvements simultanés ou de détails sans importance.
- Ne pas promettre une durée exacte, une continuité parfaite ou une résolution particulière sans réglage confirmé.

## Flux de travail

### A. Texte vers vidéo
1. Résumer l’idée en une phrase.
2. Définir sujet, action, décor, caméra et ambiance.
3. Rédiger un prompt complet en un seul bloc.
4. Vérifier les contradictions, la faisabilité visuelle et la clarté du mouvement.
5. Proposer au besoin une variante plus sobre ou plus stylisée, en ne changeant qu’un petit nombre de variables.

### B. Image vers vidéo
1. Identifier ce qui doit rester stable : identité, cadrage, vêtements, produit, décor et palette.
2. Identifier ce qui doit bouger : sujet, éléments d’arrière-plan et/ou caméra.
3. Décrire une évolution temporelle simple.
4. Éviter de demander une nouvelle composition complète si l’objectif est d’animer l’image existante.

### C. Itération après génération
Demander ce qui ne convient pas : mouvement, identité, caméra, lumière, arrière-plan ou style. Modifier seulement les éléments concernés afin de pouvoir attribuer les améliorations à une cause identifiable.

## Format de réponse par défaut

**Prompt prêt à copier**
> [Prompt final, sans commentaire intégré.]

**Intention visuelle**
- Sujet / action :
- Caméra :
- Lumière / style :
- Éléments à préserver :

**Variante (facultatif)**
Proposer une seule variante ciblée si elle apporte une réelle différence.

Ne pas afficher toutes les rubriques si une réponse courte suffit.

## Exemples

### 1. Publicité produit — texte vers vidéo

**Demande :** « Une bouteille de parfum luxueuse, publicité cinématographique. »

**Prompt :**
« Une bouteille de parfum en verre ambré, centrée sur un socle de pierre noire poli, dans un studio sombre et minimaliste. La caméra effectue un lent travelling avant avec un léger déplacement latéral, révélant progressivement les reflets sur le verre. Une lumière douce et directionnelle glisse sur les contours de la bouteille ; une brume très fine flotte à l’arrière-plan. Palette noir profond, ambre et or discret, rendu publicitaire haut de gamme, matériaux réalistes et reflets maîtrisés. La bouteille garde exactement la même forme, les mêmes proportions et la même étiquette pendant tout le plan. Fin sur un gros plan stable du produit. »

### 2. Animation d’un portrait — image vers vidéo

**Prompt :**
« Préserver le visage, la coiffure, les vêtements, le cadrage et le fond de l’image de référence. La personne cligne naturellement des yeux, respire doucement et tourne légèrement le regard vers la fenêtre, puis esquisse un petit sourire. Mouvement subtil et réaliste, caméra fixe, lumière douce et cohérente, traits du visage stables, aucune modification des vêtements ou de l’arrière-plan. »

### 3. Nature — texte vers vidéo

**Prompt :**
« Un sentier étroit traverse une forêt de pins au petit matin, avec une fine brume entre les troncs. La caméra avance lentement à hauteur d’yeux le long du sentier ; quelques branches au premier plan bougent légèrement dans la brise. Des rayons de soleil diffus traversent la brume, palette vert profond et or pâle, atmosphère contemplative, détails naturels et profondeur réaliste. Mouvement de caméra régulier, arbres et perspective cohérents, fin sur le sentier qui s’ouvre vers une clairière lumineuse. »

### 4. Mode — texte vers vidéo

**Prompt :**
« Une mannequin portant un manteau beige structuré marche à un rythme calme sur un trottoir contemporain après la pluie. Plan moyen en suivi latéral fluide, le manteau bouge naturellement à chaque pas tandis que le visage, la coupe du vêtement et ses détails restent cohérents. Reflets doux sur le sol, lumière de fin d’après-midi, esthétique éditoriale de mode, palette neutre, texture textile détaillée. Le plan se termine lorsque la mannequin s’arrête et regarde brièvement hors champ. »

## Checklist avant de livrer

- Le sujet est-il identifiable ?
- L’action est-elle visible et suffisamment précise ?
- Le mouvement du sujet et celui de la caméra sont-ils compatibles ?
- Le décor, l’éclairage et l’identité doivent-ils rester constants ?
- Le prompt décrit-il une seule séquence cohérente ?
- Les détails importants sont-ils priorisés plutôt que noyés dans des adjectifs ?
- Les options ou limites de l’interface sont-elles présentées avec prudence ?

## Source et limites

Source de départ : https://www.hunyuanvideo.org/fr/seedance25. Cette page décrit l’outil comme prenant en charge texte-vers-vidéo et image-vers-vidéo, et revendique une attention à la continuité et au mouvement. Elle précise aussi que le site est indépendant et n’est pas le site officiel Tencent Hunyuan. Ce skill est un guide de prompting pratique, pas une documentation officielle du modèle.
