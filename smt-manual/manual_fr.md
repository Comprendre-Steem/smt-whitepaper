---
header-includes:
    - \renewcommand{\contentsname}{Table of Contents}
    - \usepackage[top=3cm,bottom=3.5cm,left=4cm,right=4cm]{geometry}
urlcolor: blue
linkcolor: blue
---

# Document Metadata

* Créateurs : @ned; @theoretical
* Développeurs : @theoretical; @vandeberg; @itwasntme; @zgredek;
  @pychol-mychol; @small.minion; @youkaicountry; @picokernel
* Contributeurs : @sneak; @vandeberg; @valzav; @youkaicountry; @justinw;
  @goldibex; et al.
* Croquis : @pkattera
* Copyright (c) Steemit, Inc. 2017
* GitHub: [https://github.com/steemit/smt-whitepaper/blob/master/smt-manual/manual.md](https://github.com/steemit/smt-whitepaper/blob/master/smt-manual/manual.md)
* Traduction: @comprendre-steem (sous la supervision de @roxane)

# Smart Media Tokens (SMTs)

## Un protocole de création de tokens pour les sites web partageant du contenu, les applications, les communautés et groupes en ligne qui veulent être financés, monétisés et faire croître leur nombre d’utilisateurs.

Les Smart Media Tokens (SMT) de [Steem's](https://steem.io/steem-bluepaper.pdf) 
offrent à chacun la possibilité de lancer et de vendre ses propres tokens [Proof-of-Brain
[1]](https://steem.io/steem-bluepaper.pdf). Ces tokens sont distribués par des algorithmes basés sur des "upvote" et des "like". Ils peuvent être intégrés aux sites web pour aligner les intérêts des créateurs de ces sites sur ceux des utilisateurs et favoriser la croissance. Les sites web sont alors habilités à adopter des modèles de revenus rentables et axés sur les monnaies. Ce modèle a déjà été testé et continue de faire ses preuves sur
[steemit.com](https://steemit.com), [busy.org](https://busy.org),
[chainbb.com](https://chainbb.com), [dsound.audio](https://dsound.audio),
[dtube.video](https://dtube.video) ainsi que d’autres interfaces Steem, qui monétisent le contenu, les tokens et les médias de manière inédite.

Plusieurs protocoles connus de création de tokens, tels que l’ERC-20 d’Ethereum, permettent de créer et lancer des tokens personnalisés. Toutefois, aucun protocole ne permet aux entreprises diffusant du contenu en ligne de tirer parti de ces tokens en alignant les intérêts des utilisateurs sur ceux des applications. En effet, aucun de ces protocoles ne permettra jamais à des sites qui partagent du contenu comme Twitter, Reddit (ou les subreddits) ou le New York Times de fournir une expérience utilisateur acceptable, pour plusieurs raisons. Tout d’abord, parce que les structures imparfaites des coûts de transaction entraînent le prélèvement de frais pour des actions aussi basiques que le vote et la publication. Ensuite, parce qu’il existe une divergence d’intérêts entre les tokens principaux et secondaires qui ne sont pas conçus pour influencer la distribution en se basant sur la « Proof-of-Brain ». Enfin, parce que leurs hiérarchies de clés privées ne conviennent qu’aux opérations financières au détriment des opérations sociales et que les transactions, trop lentes, ne sont pas synchronisées avec les sites en temps réel.

Pour les sites partageant du contenu et les tokens, l’alignement des intérêts des sites web sur ceux des utilisateurs est possible grâce à l’émission constante, décentralisée et garantie mathématiquement de nouveaux tokens et à de mesures incitatives qui sont destinées aux utilisateurs (y compris les blogueurs, vlogueurs, commentateurs et curateurs). Les nouveaux tokens sont distribués selon un système de votes pondérés en fonction de l’investissement de chacun, pour éviter la triche et supprimer la nécessité d’une contrepartie. Les tokens qui sont échangés de manière sûre (grâce à des clés privées séparées pour des ensembles d’actions distincts), sans frais et en temps réel, garantissent à l’utilisateur une expérience de qualité. De plus, les entreprises qui sont capables de mobiliser des capitaux en ICO (Initial Coin Offering : émission initiale de tokens) peuvent également aligner leurs intérêts sur ceux de leurs clients. Tous les Smart Media Tokens disposent d’un support ICO intégré, au cas où l’émetteur voudrait lancer une ICO.

\tableofcontents
\newpage

# Introduction

Les Smart Media Tokens (SMT) sont une proposition visant à construire, sur la blockchain Steem, un protocole d’émission de tokens qui repose sur un consensus. Les SMT, qui s’inspirent des propriétés révolutionnaires du token STEEM (notamment la distribution automatique aux créateurs de contenu), iront encore plus loin que les protocoles blockchain d’émission de tokens créés précédemment. Cela sera rendu possible grâce à une programmabilité des ventes de tokens conçue avec soin, des fournisseurs de liquidités automatisés, des marchés de tokens décentralisés et des paramètres de distribution de tokens dynamiques, ainsi qu’un large éventail d’outils (des portefeuilles open source, des outils de signature de clés partagées, etc.) pour l’intégration dans les couches des sites web et des applications.

Les SMT font évoluer la relation fructueuse établie entre STEEM et les réseaux sociaux qui l’utilisent, tels que
[steemit.com](https://steemit.com). En moins d’un an, ce dernier s’est hissé dans le top 2 100 de l’Alexa Ranking rien qu’en intégrant le modèle incitatif de STEEM. Grâce aux SMT, n’importe quel site web ou bibliothèque de contenu sur Internet peut intégrer un ou plusieurs tokens à son interface pour faciliter la levée de fonds et la croissance autonome.

Ces tokens sont conçus pour donner une certaine flexibilité aux gestionnaires de site web lors de l’intégration du token dans leur communauté en sélectionnant des paramètres qui pourront être structurés d’emblée de façon créative ou ajustés au fil du temps. Tous les tokens lancés en tant que SMT bénéficieront d’un écosystème blockchain comportant d’une plateforme d’échange décentralisée intégrée, ainsi que d’un écosystème d’applications et de bibliothèques open source pour faciliter l’implémentation, la levée de fonds et la croissance.

## Utilisation de tokens pour une croissance autonome des utilisateurs

Les SMT sont une révolution permettant de relier toutes les applications basées sur le contenu à des tokens, alignant ainsi les intérêts des utilisateurs d’un réseau sur ceux des entrepreneurs développant les applications. Étant donné que les SMT utilisent les concepts d’inflation (l’émission de nouveaux tokens) et d’attribution de tokens via des votes attribués aux publications, les utilisateurs qui participent à leurs réseaux ou applications de contenu respectifs seront mieux récompensés. Les entrepreneurs peuvent désormais créer des tokens et les intégrer dans leur blog, application, ou dans un réseau entier d’applications et de discussions. Grâce aux SMT, ils peuvent déterminer l’aspect économique des tokens qu’ils intègrent à leurs produits, depuis les taux d’inflation jusqu’aux algorithmes de distribution des tokens.

En comparaison à d’autres tokens (comme le bitcoin, l’ether et les ERC-20), les SMT sont « intelligents et sociaux » grâce à deux caractéristiques uniques, qui permettent l’alignement des intérêts . La première est une réserve de tokens destinée à encourager la création et la curation de contenu (appelée « réserve de récompenses »). La deuxième est un système de vote qui se base sur la sagesse collective pour déterminer la valeur du contenu et lui assigner des tokens. Ces deux propriétés combinées sont appelées Proof-of-Brain, un mot dérivé de Proof-of-Work, qui met en exergue le travail humain nécessaire pour distribuer les tokens à ceux qui participent à la communauté. Le Proof-of-Brain fait des SMT un outil permettant la création de communautés en perpétuelle expansion qui encouragent leurs utilisateurs à apporter une valeur ajoutée à la communauté via une structure de récompenses intégrée.

Les entrepreneurs et les entités établies peuvent se servir des SMT pour agrandir leur réseau de partage de contenu grâce à la création automatisée et continue de nouveaux tokens qui sont attribués aux créateurs de contenu par les possesseurs des tokens existants au moyen d’un processus de vote compétitif. Comme les tokens sont distribués aux utilisateurs du réseau, les intérêts des possesseurs de tokens existants s’alignent davantage sur ceux des créateurs de contenu, des entreprises faisant fonctionner les applications et des entrepreneurs qui les soutiennent. Ces propriétés uniques incitent continuellement de nouveaux utilisateurs à rejoindre le réseau et à y participer. N’importe quelle application, qu’il s’agisse d’un mastodonte existant ou d’un réseau social en phase de test développé par une startup, pourra intégrer et utiliser ces tokens spéciaux pour s’agrandir.

## Nouvelles possibilités de levées de fonds

Les tokens reposant sur la technologie blockchain, qui ont démarré en fanfare avec l’arrivée de l’ERC20 sur Ethereum, représentent une nouvelle façon d’amener du capital dans une organisation au moyen d’une ICO. Une ICO donne l’occasion à un groupe de vendre un certain nombre de tokens initiaux, de manière publique ou privée, pour un objectif précis, dans un but commercial ou non. En fonction de la manière dont ces tokens sont vendus, les organismes de réglementation pourraient les considérer comme des produits, des titres, des produits dérivés ou les placer dans une autre catégorie encore. Quoiqu’il en soit, il est clair que plus d’un milliard de dollars américains ont été levés grâce à des ICO en 2017 et que pour s’adapter à cette tendance, le contrat ICO des SMT permet de lancer et de vendre des tokens facilement. Le lancement des SMT peut être configuré pour des ICO avec des plafonds absolus, avec des plafonds souples ou sans plafond, et peut être adapté pour recevoir du STEEM et des cryptomonnaies sur d’autres blockchains. 

## Liquidités immédiates

Grâce au concept de teneur de marché automatisé [[2](https://about.bancor.network/static/bancor_protocol_whitepaper_en.pdf)] récemment mis au point, les ICO basées sur les SMT permettent à une partie des tokens STEEM reçus d’être envoyés à un teneur de marché sur la blockchain et hors carnet de commandes afin de fournir des liquidités aux SMT à un taux de réserve spécifié. Au-delà des mécanismes sociaux et spécialisés des SMT, cette fonctionnalité renforce le concept de teneur de marché automatisé en l’associant aux marchés décentralisés des SMT, ce qui simplifie les appels d’offres et les offres de vente de la part des personnes participantes. La combinaison de ces deux marchés donne la possibilité aux teneurs de marché d’effectuer des échanges sur la blockchain qui ne sont pas basés sur la confiance, tout en assurant des liquidités pour les utilisateurs de tokens.

## Outils d'amorçage partagé

Lors de la création des SMT, les paramètres de [la réserve de récompenses](https://steem.io/steem-bluepaper.pdf) peuvent être réglés afin d’avoir une "influence partagée" entre le Steem Power et les autres SMT d’investissement, un créateur de SMT peut donc contrôler une partie de la réserve de récompenses d’un SMT pendant une période illimitée ou limitée, avec une influence croissante ou décroissante. Somme toute, l’influence partagée permet aux SMT d’être totalement ou partiellement amorcés par l’intérêt des utilisateurs existants et actifs de la communauté Steem ou d’autres SMT. Grâce à ces outils, les gestionnaires de communautés et les entrepreneurs qui lancent un token peuvent tirer parti de groupes d’utilisateurs existants pour accélérer la distribution de leur SMT à un marché cible.

## Monétisation avec des récompenses en tokens partagées

Toutes les interfaces basées sur Steem permettent de partager les récompenses en tokens entre plusieurs bénéficiaires choisis arbitrairement, qui peuvent inclure une interface, un gestionnaire de communauté, un référent, une réserve de dons pour un poste payant, etc. Une interface peut également proposer des options pour le partage des tokens entre les auteurs. Le nombre de bénéficiaires du partage de récompenses est d’abord limité à huit par les producteurs de blocs pendant que l’utilité de cette fonctionnalité est évaluée, mais la blockchain peut gérer jusqu’à 256 bénéficiaires par publication.

## Mon entité peut-elle participer aux SMT ?

Un SMT peut être lancé par une personne ou une entité. Ils ont seulement besoin d’1$ pour couvrir les frais de réseau (ces frais font en sorte qu’il y ait moins de spams et de tokens non utilisés tout en augmentant la valeur du réseau), et d’un compte sur Steem qui peut être obtenu sur [anon.steem.network](https://anon.steem.network), [steemit.com](https://steemit.com), [steemconnect.com](https://v2.steemconnect.com), ou tout autre service d’inscription Steem. 

Après obtention d’un nom de compte à l’aide duquel le token peut être enregistré, le compte crée le token en utilisant une invite de commande ou tout autre outil créé dans l’avenir pour servir au lancement de tokens. Le token peut être configuré pour permettre une vente ou une distribution initiale. Certaines propriétés d’un SMT, telles que son taux d’inflation, doivent également être définies par la personne ou l’entité qui crée le token. Ces propriétés déterminent la façon dont le token est utilisé au sein des applications et des communautés concernées.

Dès son lancement, le token devient immuable sur la blockchain et s’il est utilisé correctement, il peut avoir un effet considérable sur la croissance des entreprises qui choisissent de l’intégrer.

## Cas d’utilisation

Nous avons identifié cinq manières selon lesquelles les entreprises existantes peuvent tirer parti de SMT personnalisés pour transformer Internet. Parmi ces cas d’utilisation, vous pourrez découvrir d’autres manières de structurer et d’utiliser ces tokens dans des applications. Cette liste est loin d’être exhaustive et nous mettrons à jour ce livre blanc au fur et à mesure que d’autres cas d’utilisation montreront leur efficacité.

### 1 - Éditeurs de contenu - Utilisation d’un token unique

La croissance du site web d’un média populaire est ralentie et les créateurs du site cherchent à devancer l’évolution du paysage technologique. Le site web migre sur une application basée sur Steem ressemblant à Disqus, ou exploite directement les API de Steem pour une intégration personnalisée. Les personnes inscrites sur leur site peuvent alors être récompensées avec de la cryptomonnaie lorsqu’elles commentent. Quand le site sera prêt, ils pourront utiliser leur propre token dans l’interface de commentaires. Le token leur permettra 1) d’augmenter leur capital en vendant des tokens, 2) d’accélérer la croissance autonome.

![Single Token Content Publishers](img/uc1-Content-Publishers.png)
\begin{center}Figure 1: Publications avec token unique\end{center}

### 2 - Forums - Utilisation de tokens multiples

Une nouvelle entreprise de création de forums cherche à intégrer des cryptomonnaies dans ces derniers pour créer un flux de trésorerie et entraîner une croissance qui fasse grandir l’entreprise, mais son personnel n'est pas expert en sécurité des cryptomonnaies et préfère ne pas héberger de portefeuille de cryptomonnaies. Elle émet un SMT et l’intègre à leur site. En se concentrant uniquement sur les aspects sociaux, la société de création de forums peut intégrer d’autres applications comme SteemConnect à son forum pour prendre en charge le portefeuille et les transferts. Cela lui permet de se concentrer sur son but premier (faire grandir des communautés) sans se soucier de la sécurité de la cryptomonnaie. Le forum permet de mettre en évidence ou de lancer des tokens additionnels, pour représenter différents thèmes de discussion. Le lancement de ces tokens peut être réservé à l’entreprise à l’origine du site web ou être confié aux gestionnaires de communauté. Les tokens consacrés aux thèmes spécifiques du site entraîneront également une croissance autonome du site, niche par niche. À terme, un exemple de ce modèle multi-tokens pourrait apparaître dans des organisations telles que ChainBB ([chainbb.com](https://chainbb.com)) si cette dernière activait un token général pour l’ensemble de son domaine ainsi que des tokens ne pouvant être obtenus que dans des niches communautaires spécifiques, telles que "jardinage".

![Multiple tokens Forum](img/uc2-Forums.png)
\begin{center}Figure 2: Forum avec tokens multiples\end{center}

### 3 - Widget Commentaires pour les éditeurs en ligne

L’un des moyens d’encourager les éditeurs de contenus à utiliser les SMT est de fournir un widget "Commentaires" basé sur Steem qui peut être facilement intégré sur les blogs existants sur les logiciels tels que WordPress et Blogger. Le développeur qui utilise le widget pourra percevoir un pourcentage des tokens (qu’on appelle les "récompenses partagées") distribués aux personnes qui écrivent les commentaires. ll y a donc une opportunité commerciale pour une prochaine génération d’entreprises comme Disqus utilisant la cryptomonnaie. Cela permettrait d’alléger la contrainte de la signature des transactions, de la gestion des clés privées, de la fonctionnalité du portefeuille et des coûts d’hébergement pour l’éditeur. Comment ? En déléguant toutes ces fonctions au gestionnaire du widget Commentaires.

![Comment Widget](img/uc3-Comment-Widget.png)
\begin{center}Figure 3: Widget de commentaire\end{center}

### 4 - Modérateurs et gestionnaires de sous-communautés

Imaginez que vous êtes modérateur pour un thème spécifique dans un forum, comme un « subreddit » sur Reddit ou une « communauté » sur Steemit. Si un site web intègre des SMT pour des thèmes spécifiques, alors les modérateurs responsables de ces thèmes peuvent lancer ces tokens pour dynamiser les abonnés à leur thème, lever des fonds et améliorer la qualité de la curation de contenu pour la communauté.

![Sub-community](img/uc4-subcommunity.png)
\begin{center}Figure 4: Sous-communauté\end{center}

### 5 - Ressources arbitraires - Tokens représentant des ressources réelles

Examinons une situation dans laquelle un entrepreneur cherche à fournir des liquidités dans l’écosystème Steem. Celui-ci peut émettre un SMT ne subissant pas d’inflation et le structurer de manière à lier son prix à celui du dollar (ou autre dette, contrat ou ressource), ce qui le rend analogue à une reconnaissance de dette ou à un produit dérivé basique. La structure du SMT prévoit, entre autres, que celui-ci soit vendu à environ 1$, d’une manière similaire au Tether. L’entrepreneur met en place une fonctionnalité permettant les virements bancaires pour l’achat et la vente et prélève une petite commission sur chaque transaction. Le produit dérivé est échangé contre du STEEM et fait rentrer des capitaux dans l’écosystème, qui peuvent être utilisés par tous les tokens.

![IOU Asset Token Exchange](img/uc5-IOU-assets.png)
\begin{center}Figure 5: Marché d'échange pour ressources réeles\end{center}

# Mode d’emploi

Ce manuel explique le fonctionnement des SMT dans les moindres détails. Il se destine aux utilisateurs techniques qui veulent créer leurs propres SMT.

## Créer un compte de contrôle

Pour créer un SMT, il faut en premier lieu lui créer un compte de contrôle. N’importe quel compte STEEM peut servir de compte de contrôle, mais il est fortement recommandé de créer un compte spécialement prévu à cet effet. Il est également fortement recommandé de ne pas utiliser ce compte pour publier, voter, ou contenir des STEEM, SBD ou autres tokens (excepté un petit montant de STEEM investis pour la bande passante des transactions).

Le nom du compte de contrôle n’aura qu’une faible visibilité dans la plupart des interfaces utilisateur. En conséquence, ce n’est pas très grave si ce nom n’est pas celui qui convient le mieux pour le nom du SMT.

### Sécurité du compte de contrôle

La sécurité sur le compte de contrôle est importante pour ceux qui désirent utiliser le compte après le lancement.

- Le compte de contrôle devrait utiliser une sécurité multisignatures de type 2-sur-3 ou 3-sur-5.
- Les signatures sur le compte devraient être d’autres comptes, et non des clés spécifiques.
- Pour davantage de sécurité, les comptes qui font partie du groupe de multisignatures du compte de contrôle devraient eux aussi utiliser une sécurité multisignatures.
- Un sous-ensemble de clés devrait être gardé hors ligne, dans des machines air gap.
- Les transactions devraient être générées via une interface en ligne, et transférées physiquement vers les machines air gap via des disques amovibles.
- Les signatures devraient être remises sur le système en ligne via des disques amovibles physiques pour la transmission via l’interface utilisateur.

Il est évident qu’une fois que les signatures ont été programmées, il faudrait vérifier que le compte est toujours capable d’opérer des transactions. Il est recommandé de tester vos paramètres de signature et de signature de transaction en utilisant un testnet, ou un compte moins important sur le réseau principal.

Une fois que le token a été lancé, vous devriez penser à détruire les clés du compte en les envoyant à @null, ce qui lance un token pour lequel les propriétés dynamiques ne peuvent jamais être modifiées.

### Consensus sur les tokens

Étant donné que les tokens participent à d'infimes transactions (qui ont aussi une influence sur les STEEM), ils sont conçus comme faisant partie du consensus dans la blockchain Steem.

## Création de tokens et paramètres initialisés

### Création de SMT

La première opération qui doit être effectuée est `smt_create_operation`. Cette opération crée un SMT dans la blockchain. Après avoir exécuté `smt_create_operation`, le SMT nouvellement créé n’est pas encore totalement configuré. 

Cette configuration a lieu en grande partie lors des opérations suivantes :
`smt_set_setup_parameters_operation`, `smt_setup_inflation_operation` et
`smt_setup_operation`. Ces opérations peuvent avoir lieu dans la même transaction ou à n’importe quel autre moment ultérieur.

```
struct smt_create_operation
{
   account_name_type control_account;
   asset             smt_creation_fee;
   asset_symbol_type symbol;
   extensions_type   extensions;
};
```

#### Identificateurs d’actifs numériques

Un SMT est déterminé par un *identificateur d’actif numérique* (IAN), qui consiste en deux signes arobase suivis de neuf chiffres décimaux, par exemple `@@314159265`. La blockchain impose que l’identificateur mis en place par une interface utilisateur dans `smt_create_operation` corresponde au résultat de l’appel de procédure à distance (RPC) de `get_next_smt_identifier`. C’est pourquoi un IAN ne peut pas être choisi au hasard par le créateur du SMT. Il n’est même pas possible de "miner" un "IAN personnalisé" (en référence aux "adresses Bitcoin personnalisées" que certaines personnes utilisent).

La raison de cette restriction est que les créateurs de la blockchain veulent décourager les utilisateurs de se servir des identificateurs consensuels comme de noms de symbole, pour qu’ils utilisent plutôt un registre système non consensuel afin de relier des symboles ayant du sens pour tout un chacun à des actifs. La blockchain ne peut pas distinguer un cyber-squatteur du propriétaire légitime d’une marque, surtout si le squatteur est prêt à payer des frais de création de SMT.

#### Nommer les SMT

Pour éviter que certaines personnes squattent des noms, il faut publier un registre d’actifs qui associe des IAN aux noms. Un registre d’actifs ne repose pas sur un consensus. Cela signifie que toutes les opérations de la blockchain ne sont numérotées que grâce aux IAN. Les noms des actifs ne sont utilisés que pour la présentation de l’interface utilisateur.

Une interface utilisateur peut comporter un registre d’actifs sous la forme d’un fichier, d’une URL ou d’un compte blockchain qui publie les entrées du registre avec des opérations personnalisées. Celui qui publie un registre d’actifs devrait s’assurer que les entrées du registre sont conformes aux normes légales de propriété de marque qu’il décide d’appliquer.

#### Frais de création des SMT

Pour lancer une `smt_create_operation`, il faut payer un `smt_creation_fee`. Le montant requis est défini par le champ `smt_creation_fee` de `dynamic_global_properties_object`. Ce champ peut contenir une valeur en STEEM ou en SBD. Si cette valeur est en SBD, un montant équivalent de STEEM sera accepté, au taux de change du moment.

Le `smt_creation_fee` initial sera fixé à 1 SBD, et rien ne sera fait pour le mettre à jour. Il est toutefois possible que le montant du `smt_creation_fee` soit modifié dans les futurs hard forks, les utilisateurs-agents devraient donc lire la valeur du `smt_creation_fee` à partir du `dynamic_global_properties_object`. Les agents utilisateurs ne doivent pas s’attendre à ce que ce prix reste à 1 SBD et peuvent être amenés à réclamer des frais supplémentaires si l’objectif de l’interface est de ne permettre qu’un ensemble de tokens faisant l’objet d’une curation.

Envoyer cette somme à `STEEM_NULL_ACCOUNT` la détruira.

### Préréglage des SMT 

Deux opérations de préréglage sont comprises : `smt_setup_inflation_operation` et `smt_setup_parameters`. Ces opérations doivent avoir lieu après la `smt_create_operation`, et avant la `smt_setup_operation`. Elles peuvent avoir lieu dans la même transaction, ou dans les blocs précédents.

La raison pour laquelle les opérations de préréglage ne font pas partie de `smt_setup_operation`
est que cela permet à un grand nombre d’opérations de préréglage d’être exécutées sur plusieurs blocs.

### Réglage des SMT

Chaque SMT possède un descripteur associé dont *les données de configuration sont permanentes*. Ces données ne peuvent être modifiées après la mise sur le marché du SMT ! Le descripteur est programmé grâce à `smt_setup_operation`:

```
struct smt_setup_operation
{
   account_name_type       control_account;
   asset_symbol_type       smt_name;
   int64_t                 max_supply = STEEM_MAX_SHARE_SUPPLY;

   smt_generation_policy   initial_generation_policy;

   time_point_sec          generation_begin_time;
   time_point_sec          generation_end_time;
   time_point_sec          announced_launch_time;
   time_point_sec          launch_expiration_time;

   extensions_type         extensions;
};
```

L’exactitude de la `smt_setup_operation` fait autorité. Elle diffère peut-être de l’exactitude de toute opération spécifiée précédente, et elle la supplantera à l’avenir. Les opérations exécutées ultérieurement doivent avoir une exactitude correspondante.

L’opération doit être signée par la clé du `control_account` (compte de contrôle). Il faut que les SMT aient été créés au préalable par le `control_account`. Les décimales intégrées au symbole peuvent être différentes de la `smt_setup_operation` précédente.

Le champ `decimal_places` est utilisé par les interfaces utilisateur pour afficher les unités comme un nombre de décimales.

Le `generation_begin_time` est la période au cours de laquelle les participants peuvent commencer à contribuer à l’ICO. Ce sera permis à l’avenir. Dès lors, les utilisateurs auront le temps d’étudier les conditions finales des ICO avant leur début. 

Le `generation_end_time` est la période où l’ICO n’accepte plus les contributions, et le `announced_launch_time` est le moment où les tokens de l’ICO sont créés (en partant du principe que l’ICO a atteint le niveau minimum de participation). Il y a une certaine période de transition entre le `generation_end_time` et le `announced_launch_time` pour donner la possibilité d’effectuer des ICO dont les plafonds, cachés, ne sont pas dévoilés au moment où l’ICO accepte les contributions. Cela donne également le temps au créateur de l’ICO d’utiliser les chiffres définitifs de l’ICO pour soutenir ses activités commerciales préalablement au lancement.

Au moment du `launch_expiration_time`, si l’ICO n’a pas encore été lancée, tous les contributeurs sont totalement remboursés (par le biais d’opérations virtuelles) et l’ICO est annulée. Le logo reste réservé au `control_account`. spécifié. Cependant, pour pouvoir lancer le token, il faut exécuter une `smt_create_operation` et il faut payer les frais de création des SMT, `smt_creation_fee` , une nouvelle fois.

### Unités de token

La création initiale de tokens est possible grâce à un don d’unités STEEM de la part des contributeurs. Pour éviter des problèmes d’arrondissement, le don doit être un nombre entier d’unités STEEM. Le créateur de l’ICO définit la taille d’une unité STEEM, qui peut être petite ou grande. Il vaut mieux utiliser une petite unité ( 1 STEEM ou 0,1 STEEM, par exemple), car cela permet à l’ICO d’être accessible à un public aussi large que possible.

Une unité STEEM suit aussi une politique de routage qui détermine où vont les STEEM au lancement du token. (Les STEEM des tokens qui n’ont pas été lancés pourront être remboursés, sur demande.) Cette politique de routage peut diviser les STEEM contenus dans l’unité et les répartir entre plusieurs parties.

Quand l’ICO a lieu, les tokens sont créés en *unités de token*. Plusieurs unités de token sont créées par unité de STEEM mise à contribution. Les unités de token suivent également une politique de routage.

Les unités et leurs politiques de routage sont spécifiées dans la structure `smt_generation_unit` :

```
struct smt_generation_unit
{
   flat_map< account_name_type, uint16_t >        steem_unit;
   flat_map< account_name_type, uint16_t >        token_unit;
};
```

Chaque paire `(key, value)` dans la `flat_map` détermine le routage de certains satoshis. Le total des STEEM/tokens dans chaque unité est simplement la somme des valeurs.

### Taux unitaires

Quand un SMT est lancé, des unités de token sont créées pour les unités de STEEM à un taux de R-pour-1. Le nombre correspondant à la lettre R est le *taux unitaire*. Les valeurs minimum et maximum allouables à R sont spécifiées respectivement dans les champs `min_unit_ratio` et `max_unit_ratio` de `smt_generation_policy`.

Le nombre maximum d’unités de token qui peuvent être créées grâce à l’ICO est limité par `max_token_units_generated`, un paramètre mis en place par le créateur de l’ICO. (Il est possible de créer plus de tokens après le lancement du token, mais cette création "tardive" est appelée *inflation* et n’est pas considérée comme faisant partie de l’ICO.)

Le taux unitaire est défini au plus grand nombre entier qui ne résulterait pas en un `max_token_units_generated` excédentaire pour le nombre d’unités de STEEM réellement utilisées.

### Plafond et minimum

Les ICO peuvent définir un nombre minimum d’unités STEEM `min_steem_units`. Si l’ICO n’atteint pas `min_steem_units` avant `generation_end_time`, alors l’ICO n’aura pas lieu, et les contributeurs auront droit à un remboursement.

Les ICO peuvent également définir deux nombres maximum d’unités STEEM: un *plafond absolu* (*hard cap*) et un *plafond souple* (*soft cap*). Pour les unités qui dépassent le plafond souple, le routage est différent pour les STEEM et les tokens. Les unités STEEM qui dépassent le plafond absolu sont rejetées et ne génèrent aucun SMT.

Les effets du plafond souple sont divisés proportionnellement entre tous les contributeurs. Cela veut dire que si une ICO a un plafond souple de 8 millions de STEEM et que 10 contributeurs investissent 1 million de STEEM, alors 0,2 million des STEEM de chaque utilisateur est routé via la politique du plafond souple. 

Les effets du plafond absolu ne sont ressentis que par les derniers contributeurs. Cela veut dire que si une ICO a un plafond absolu de 8 millions de STEEM, et que 10 contributeurs investissent chacun 1 million de STEEM, alors les 8 premiers utilisateurs ont participé complètement à l’ICO et les 2 derniers seront remboursés de 1 million de STEEM.

### Plafonds cachés

Les plafonds minimum et absolu sont cachés dans la politique de production. Cela signifie que ces montants sont fixés au moment de la configuration, mais le créateur de l’ICO a la possibilité de les garder secrets. Cette fonctionnalité est mise en œuvre par un protocole cryptographique de mise en gage : un hash appelé mise en gage est publié au moment de la configuration et le montant réel doit correspondre à la mise en gage. (Un nonce est également compris dans le hash pour empêcher tout pirate de trouver le plafond caché en faisant des suppositions.)

Le créateur du SMT pourrait vouloir prépublier une garantie que les valeurs cachées sont comprises dans une certaine plage. Les champs `lower_bound` et `upper_bound` permettent cette fonctionnalité : un montant révélé qui n’est pas dans la plage indiquée est traité de la même manière qu’une erreur de hachage. 

```
struct smt_cap_commitment
{
   share_type            lower_bound;
   share_type            upper_bound;
   digest_type           hash;
};

struct smt_revealed_cap
{
   share_type            amount;
   uint128_t             nonce;
};

struct smt_cap_reveal_operation
{
   account_name_type     control_account;
   smt_revealed_cap      cap;

   extensions_type       extensions;
};
```

Tous les plafonds sont cachés, mais le plafond peut être révélé à n’importe quel moment. Ainsi, une ICO dont le plafond ou le minimum n’est pas dissimulé peut être mise en place. Il suffit d’ajouter `smt_cap_reveal_operation` dans la même opération que `smt_setup_operation`. Les interfaces utilisateurs doivent permettre des fonctionnalités à cet effet. 

Une interface utilisateur devrait mettre en place une ou plusieurs des mesures suivantes pour s’assurer que le `nonce` et le `amount` soient récupérables.

- Forcer l’utilisateur à entrer à nouveau le amount et le nonce, pour confirmer qu’ils ont été sauvegardés. 
- Définir le `nonce` comme une fonction déterministe de la clé privée et des données publiques, par exemple `nonce = H(privkey + control_account + lower_bound +
  upper_bound + current_date)`.
- Fournir une fonctionnalité pour brute-forcer les champs incertains quand le nonce est connu (par exemple, la date du jour et le `amount`).
- Prévoir un montant avec une faible entropie pour simplifier le brute-forcing quand le nonce est connu (par exemple, un nombre entre 1 et 999 fois une puissance de 10) .

### Structure des données de la stratégie de création

La structure de la stratégie de création des SMT ressemble à ça :

```
struct smt_capped_generation_policy
{
   smt_generation_unit pre_soft_cap_unit;
   smt_generation_unit post_soft_cap_unit;

   smt_cap_commitment  min_steem_units_commitment;
   smt_cap_commitment  hard_cap_steem_units_commitment;

   uint16_t            soft_cap_percent = 0;

   uint32_t            min_unit_ratio = 0;
   uint32_t            max_unit_ratio = 0;

   extensions_type     extensions;
};
```

Remarque, le paramètre `max_token_units_generated` n’apparaît nulle part dans l’opération. La raison est qu’il s’agit en réalité d’un paramètre dérivé : `max_token_units_generated = min_unit_ratio * hard_cap_steem_units`.

De plus, la `smt_generation_policy` est définie comme étant une `static_variant`,
dont la `smt_capped_generation_policy` est l’unique membre:

```
typedef static_variant< smt_capped_generation_policy > smt_generation_policy;
```

Ce `typedef` pourra permettre aux prochaines versions du protocole d’accepter des sémantiques de stratégie de création supplémentaires avec différents paramètres. 

### Exemples et argumentation

#### Exemple de l’ICO

ALPHA veut vendre un token au public pour récolter des fonds : 70 % des STEEM investis vont sur le compte de l’organisation Alpha (@alpha_org), 23 % sur le compte du fondateur A (@founder_a) et 7 % sur le compte du fondateur B (@founder_b).

ALPHA définit une unité STEEM comme suit :

```
steem_unit = [["alpha_org", 70], ["founder_a", 23], ["founder_b", 7]]
```

Cette unité STEEM contient 100 STEEM-satoshis, ou 0,1 STEEM.

Pour chaque STEEM investi, un investisseur dans ALPHA recevra 5 tokens ALPHA, et le compte du fondateur D recevra 1 token ALPHA. Ce rapport ⅚ - ⅙ s’exprime de la manière suivante : 

```
token_unit = [["$from", 5], ["founder_c", 1]]
```

Ce rapport est défini dans la structure de données suivante :

```
struct smt_generation_unit
{
   flat_map< account_name_type, uint16_t >        steem_unit;
   flat_map< account_name_type, uint16_t >        token_unit;
};
```

Cette unité de token contient 6 ALPHA-satoshis, ou 0,0006 Alpha ( si les ALPHA acceptent 4 décimales).

Ensuite, nous définissons le *taux unitaire* comme étant le taux relatif auquel les `token_unit` sont émis à mesure que les `steem_unit` sont investis. Pour correspondre à ce prérequis de 6 ALPHA pour 1 STEEM, il faut émettre 1000 unités ALPHA par unité STEEM. C’est pourquoi le taux unitaire de cette ICO est de 1000. Le taux unitaire est placé dans les champs `min_unit_ratio` et `max_unit_ratio` de la structure de données 
`smt_capped_generation_policy` :

```
min_unit_ratio = 1000
max_unit_ratio = 1000
```

Un nom de compte spécial, `$from`, représente l’investisseur. Il existe également des comptes `$from.vesting`, qui représentent le montant bloqué par le compte `$from`.

#### Pourquoi les taux unitaires ?

Pourquoi la blockchain utilise-t-elle des taux unitaires plutôt que de simplement spécifier les prix ?

La réponse est qu’il est possible d’écrire des définitions d’ICO pour lesquelles le prix est mal défini. Par exemple :

- `"$from"` n’est pas présent dans `token_unit`.
- `"$from"` est présent à la fois dans `token_unit` et `steem_unit`.
- Une combinaison de `"$from"` et `"$from.vesting"` est présente.
- L’expansion à l’avenir permet la création de nouveaux comptes spéciaux.

Toutes ces définitions d’ICO ont un taux unitaire, mais définir une quantité unique que l’on puisse qualifier de « prix » est compliqué, voire impossible pour ce genre d’ICO.

#### Traitement des taux unitaires par l’interface utilisateur

Du fait de ce qui précède, le concept de "prix d’ICO" ne s’applique qu’au niveau de l’interface utilisateur. Les interfaces qui affichent un prix d’ICO doivent suivre les règles suivantes :

- Donner une définition précise du "prix" affiché par l’interface.
- Pouvoir fonctionner correctement en recevant des entrées problématiques comme celles mentionnées ci-dessus.
- Comporter un bouton permettant de passer de l’affichage du taux unitaire à l’affichage du prix.

#### FAQ sur les plafonds cachés

- Q: Mon ICO doit-elle avoir un plafond ?
- R: Certaines personnes sont repoussées par les ICO non plafonnées, car celles-ci semblent relever d’une certaine "cupidité", ou veulent une garantie quant au pourcentage minimum de l’ICO que leur contribution leur permettra de posséder. Si vous voulez que ces personnes participent, définissez un plafond.

- Q: Mon plafond doit-il être caché ?
- R: Certaines personnes aiment la transparence et la certitude qui vont de pair avec un plafond public. D’autres considèrent qu’un plafond secret est plus motivant et crée de la demande. L’un des compromis possibles est de rendre publiques les puissances de 10 entre lesquelles le plafond est compris, par exemple Le plafond de cette ICO est compris entre 1 million et 10 millions de STEEM.

- Q: Comment désactiver le plafond ?
- R: Paramétrez le plafond de façon à ce qu’il soit supérieur à `STEEM_MAX_SHARE_SUPPLY`.

### Lancement

La *période de lancement effective* est la période au cours de laquelle les tokens deviennent transférables. Il y a deux possibilités en fonction du moment où le plafond absolu est révélé :

- Lorsque les `min_steem_units` et les `hard_cap_steem_units` sont révélées avant le `announced_launch_time`, le lancement est qualifié de *lancement ponctuel*. La logique du lancement est exécutée par la blockchain dès que l’`announced_launch_time` est arrivé, qu’importe les autres actions des utilisateurs.
- Lorsque les `min_steem_units` et les `hard_cap_steem_units` ne sont pas révélées avant le `announced_launch_time`, le lancement est qualifié de *lancement retardé*. La logique du lancement est exécutée par la blockchain lorsque les `min_steem_units` et les `hard_cap_steem_units` ont été révélées.
- Si le lancement est retardé, tous les investisseurs peuvent utiliser la `smt_refund_operation` pour récupérer leurs STEEM à n’importe quel moment après le `announced_launch_time`, et avant que la logique de lancement ne soit exécutée.

Les raisons de cette conception sont les suivantes :

- Le plafond dissimulé n’est pas publié dans l’immédiat (c’est la définition de *dissimulé*).
- Publier le plafond dissimulé est une action qui doit être menée par le créateur de l’ICO (encore une fois, toute action qui requiert des informations non publiques ne peut avoir lieu automatiquement dans la blockchain).
- Si le créateur de l’ICO ne fait rien, la logique de lancement ne sera jamais exécutée. 
- Un créateur d’ICO peut être malintentionné ou passif. Dans ce cas, les personnes qui ont investi des STEEM seront bel et bien piégées à jamais et ne recevront jamais aucun token.
- Pour empêcher que des STEEM ne soient piégés de cette façon, il existe l’opération `smt_refund_operation`.

```
struct smt_refund_operation
{
   account_name_type       contributor;
   asset                   amount;
   extensions_type         extensions;
};
```

Remarque : les utilisateurs ne sont pas *obligés* d’utiliser la `smt_refund_operation`; chaque investisseur individuel choisit de recevoir un remboursement. Si le créateur de l’ICO annonce une raison légitime de l’échec de l’émission avant le `announced_launch_time`, , il est possible que tous ou la majorité des investisseurs choisissent de leur plein gré de ne pas utiliser la `smt_refund_operation`. Dans ce cas, le lancement aura lieu dès que le créateur de l’ICO aura publié les valeurs cachées.

La logique de lancement considère un investissement suivi d’un remboursement comme étant une absence totale d’investissement. C’est pourquoi, quand un lancement a lieu avec du retard, chaque investisseur se retrouvera *exactement dans un* de ces deux états:

- L’investisseur a exécuté la `smt_refund_operation`, a reçu le remboursement de ses STEEM et ne participe pas à l’ICO.
- L’investisseur n’a pas fait appel à un remboursement, il participe à l’ICO.

Il est possible qu’un lancement retardé ait excédé la valeur `min_steem_units` au moment annoncé du lancement, mais qu’il retombe par la suite sous la valeur `min_steem_units` à cause des remboursements. Dans ce cas, l’ICO n’aura pas lieu. Elle sera traitée comme si elle n’avait jamais atteint le `min_steem_units`.

### Exemples complets en JSON

#### ALPHA

Cet exemple est basé sur l’exemple ALPHA cité plus haut. Cette ICO a les caractéristiques suivantes : 

- 70 % des STEEM engagés vont au compte de l’organisation Alpha (@alpha_org).
- 23 % des STEEM engagés vont au compte fondateur A (@founder_a).
- 7 % des STEEM engagés vont au compte fondateur B (@founder_b).
- La contribution unitaire minimum est de 0,1 STEEM.
- Pour chaque STEEM engagé, le contributeur reçoit 5 ALPHA (@contributor_a).
- Pour chaque STEEM engagé, le compte fondateur C reçoit 1 ALPHA (@founder_c).
- Pas de minimum, pas de plafond souple ni de plafond absolu.
- Aucune inflation post-lancement.

![Alpha ICO example](img/ico-example-alpha.png)
\begin{center}Figure 6: ICO Alpha\end{center}

Voici les opérations pour le lancement d’ALPHA :

```
[
 ["smt_setup",
  {
   "control_account" : "alpha",
   "decimal_places" : 4,
   "max_supply" : "1000000000000000",
   "initial_generation_policy" : [0,
    {
     "pre_soft_cap_unit" : {
      "steem_unit" : [["alpha_org", 70], ["founder_a", 23], ["founder_b", 7]],
      "token_unit" : [["$from", 5], ["founder_c", 1]]
     },
     "post_soft_cap_unit" : {
      "steem_unit" : [],
      "token_unit" : []
     },
     "min_steem_units_commitment" : {
      "lower_bound" : 1,
      "upper_bound" : 1,
      "hash" : "32edb6022c0921d99aa347e9cda5dc2db413f5574eebaaa8592234308ffebd2b"
     },
     "hard_cap_steem_units_commitment" : {
      "lower_bound" : "166666666666",
      "upper_bound" : "166666666666",
      "hash" : "93c5a6b892de788c5b54b63b91c4b692e36099b05d3af0d16d01c854723dda21"
     },
     "soft_cap_percent" : 10000,
     "min_unit_ratio" : 1000,
     "max_unit_ratio" : 1000,
     "extensions" : []
    }
   ],
   "generation_begin_time" : "2017-08-10T00:00:00",
   "generation_end_time" : "2017-08-17T00:00:00",
   "announced_launch_time" : "2017-08-21T00:00:00",
   "smt_creation_fee" : "1.000 SBD",
   "extensions" : []
  }
 ],
 ["smt_cap_reveal",
  {
   "control_account" : "alpha",
   "cap" : { "amount" : 1, "nonce" : "0" },
   "extensions" : []
  }
 ],
 ["smt_cap_reveal",
  {
   "control_account" : "alpha",
   "cap" : { "amount" : "166666666666", "nonce" : "0" },
   "extensions" : []
  }
 ]
]
```

Quelques remarques : 

- Le plafond souple est désactivé en réglant la valeur de `soft_cap_percent` à
  `STEEM_100_PERCENT = 10000`.
- `post_soft_cap_unit` doit être vide quand le plafond souple est désactivé.
- Le taux unitaire ne change pas, donc les `min_unit_ratio` / `max_unit_ratio` doivent être définis en conséquence.
- Les plafonds secrets sont désactivés en utilisant un nonce égal à zéro et en paramétrant `lower_bound
  == upper_bound`.
- Les plafonds doivent encore être révélés via `smt_cap_reveal_operation`.
- Le plafond absolu spécifié est le plafond absolu le plus élevé possible sans entraîner la création d’un nombre de tokens dépassant `STEEM_MAX_SHARE_SUPPLY`.

#### BETA

Les tokens BETA sont créés selon les règles suivantes :

- À chaque fois que 5 STEEM sont investis, 3 STEEM sont attribués au compte fondateur de Fred.
- À chaque fois que 5 STEEM sont investis, 2 STEEM sont attribués au compte fondateur de Georges.
- 10 % de la réserve des tokens initiaux reviennent au compte fondateur de Georges.
- 20 % de la réserve des tokens initiaux reviennent au compte fondateur de Henri.
- 70 % de la réserve de tokens initiaux sont partagés entre les investisseurs proportionnellement à leurs investissements.
- Chaque unité de STEEM correspond à 0,005 STEEM.
- Chaque unité de token correspond à 0,0010 BETA.
- Le minimum de fonds récoltés est de 5 millions d’unités STEEM, soit 25 000 STEEM.
- Le maximum de fonds récoltés est de 30 millions d’unités STEEM, soit 150 000 STEEM.
- Chaque investisseur reçoit entre 7 et 14 BETA par STEEM investi, en fonction de la totalité des investissements.
- Georges reçoit entre 1 et 2 BETA par STEEM investi, en fonction de la totalité des investissements.
- Henri reçoit entre 2 et 4 BETA par STEEM investi, en fonction de la totalité des investissements.
- Si la somme maximum de 30 millions d’unités de STEEM est atteinte, alors l’équation `min_unit_ratio
  = 50` s’applique.
- Le nombre maximum d’unités de token équivaut à `min_unit_ratio` multiplié par 30 millions, soit 1,5 milliard d’unités de token.
- Vu que chaque unité équivaut à 0,0010 BETA, 1,5 million de tokens BETA au maximum seront créés.
- Si 75 000 STEEM ou moins sont investis, les investisseurs Georges et Henri recevront un maximum de 14, 2 et 4 BETA par STEEM investi (respectivement).
- Si plus 75 000 STEEM sont investis, George et Henri recevront des BETA à un taux de 70 % / 10 % / 20 %, de manière à ce que le total soit fixé à 1,5 million de BETA.
- Vu le plafond absolu, Georges et Henri reçoivent au moins 7, 1 et 2 BETA par STEEM investi (respectivement).

Cet exemple est choisi pour montrer comment les taux fonctionnent. Ce n’est pas un exemple réaliste. En effet, la plupart des ICO décident soit d’appliquer `min_unit_ratio = max_unit_ratio` comme ALPHA, soit d’utiliser un taux `max_unit_ratio` élevé, comme BETA.

```
[
 [
  "smt_setup",
  {
   "control_account" : "beta",
   "decimal_places" : 4,
   "max_supply" : "1000000000000000",
   "initial_generation_policy" : [0,
    {
     "pre_soft_cap_unit" : {
      "steem_unit" : [["fred", 3], ["george", 2]],
      "token_unit" : [["$from", 7], ["george", 1], ["henry", 2]]
     },
     "post_soft_cap_unit" : {
      "steem_unit" : [],
      "token_unit" : []
     },
     "min_steem_units_commitment" : {
      "lower_bound" : 5000000,
      "upper_bound" : 5000000,
      "hash" : "dff2e4aed5cd054439e045e1216722aa8c4758b22df0a4b0251d6f16d58e0f3b"
     },
     "hard_cap_steem_units_commitment" : {
      "lower_bound" : 30000000,
      "upper_bound" : 30000000,
      "hash" : "f8e6ab0e8f2c06a9d94881fdf370f0849b4c7864f62242040c88ac82ce5e40d6"
     },
     "soft_cap_percent" : 10000,
     "min_unit_ratio" : 50,
     "max_unit_ratio" : 100,
     "extensions" : []
    }
   ],
   "generation_begin_time" : "2017-06-01T00:00:00",
   "generation_end_time" : "2017-06-30T00:00:00",
   "announced_launch_time" : "2017-07-01T00:00:00",
   "smt_creation_fee" : "1000.000 SBD",
   "extensions" : []
  }
 ],
 [
  "smt_cap_reveal",
  {
   "control_account" : "beta",
   "cap" : { "amount" : 5000000, "nonce" : "0" },
   "extensions" : []
  }
 ],
 [
  "smt_cap_reveal",
  {
   "control_account" : "beta",
   "cap" : { "amount" : 30000000, "nonce" : "0" },
   "extensions" : []
  }
 ]
]
```

[Cette feuille de calcul](ico-parameters.ods) permet de clarifier ce rapport.

#### GAMMA

Le token GAMMA est comme le BETA, à une différence près : le `max_unit_ratio` élevé signifie que le nombre maximum de tokens, 1,5 million, est atteint très rapidement lors de l’ICO. En résumé, l’ICO suivante répartit 1,5 million de tokens GAMMA entre les contributeurs (à condition qu’au moins 5 STEEM soient engagés).

```
[
 [
  "smt_setup",
  {
   "control_account" : "gamma",
   "decimal_places" : 4,
   "max_supply" : "1000000000000000",
   "initial_generation_policy" : [0,
    {
     "pre_soft_cap_unit" : {
      "steem_unit" : [["fred", 3], ["george", 2]],
      "token_unit" : [["$from", 7], ["george", 1], ["henry", 2]]
     },
     "post_soft_cap_unit" : {
      "steem_unit" : [],
      "token_unit" : []
     },
     "min_steem_units_commitment" : {
      "lower_bound" : 5000000,
      "upper_bound" : 5000000,
      "hash" : "dff2e4aed5cd054439e045e1216722aa8c4758b22df0a4b0251d6f16d58e0f3b"
     },
     "hard_cap_steem_units_commitment" : {
      "lower_bound" : 30000000,
      "upper_bound" : 30000000,
      "hash" : "f8e6ab0e8f2c06a9d94881fdf370f0849b4c7864f62242040c88ac82ce5e40d6"
     },
     "soft_cap_percent" : 10000,
     "min_unit_ratio" : 50,
     "max_unit_ratio" : 300000,
     "extensions" : []
    }
   ],
   "generation_begin_time" : "2017-06-01T00:00:00",
   "generation_end_time" : "2017-06-30T00:00:00",
   "announced_launch_time" : "2017-07-01T00:00:00",
   "smt_creation_fee" : "1000.000 SBD",
   "extensions" : []
  }
 ],
 [
  "smt_cap_reveal",
  {
   "control_account" : "gamma",
   "cap" : { "amount" : 5000000, "nonce" : "0" },
   "extensions" : []
  }
 ],
 [
  "smt_cap_reveal",
  {
   "control_account" : "gamma",
   "cap" : { "amount" : 30000000, "nonce" : "0" },
   "extensions" : []
  }
 ]
]
```

#### DELTA

Dans l’ICO suivante, un million de tokens DELTA sont créés pour le fondateur et aucun n’est créé pour les contributeurs. Une petite contribution de 0,1 STEEM peut être donnée par n’importe quel utilisateur (y compris les fondateurs eux-mêmes) pour déclencher la création.

```
[
 [
  "smt_setup",
  {
   "control_account" : "delta",
   "decimal_places" : 5,
   "max_supply" : "1000000000000000",
   "initial_generation_policy" : [0,
    {
     "pre_soft_cap_unit" : {
      "steem_unit" : [["founder", 1]],
      "token_unit" : [["founder", 10000]]
     },
     "post_soft_cap_unit" : {
      "steem_unit" : [],
      "token_unit" : []
     },
     "min_steem_units_commitment" : {
      "lower_bound" : 10000000,
      "upper_bound" : 10000000,
      "hash" : "4e12522945b8cc2d87d54debd9563a1bb6461f1b1fa1c31876afe3514e9a1511"
     },
     "hard_cap_steem_units_commitment" : {
      "lower_bound" : 10000000,
      "upper_bound" : 10000000,
      "hash" : "4e12522945b8cc2d87d54debd9563a1bb6461f1b1fa1c31876afe3514e9a1511"
     },
     "soft_cap_percent" : 10000,
     "min_unit_ratio" : 1000,
     "max_unit_ratio" : 1000,
     "extensions" : []
    }
   ],
   "generation_begin_time" : "2017-06-01T00:00:00",
   "generation_end_time" : "2017-06-30T00:00:00",
   "announced_launch_time" : "2017-07-01T00:00:00",
   "smt_creation_fee" : "1000.000 SBD",
   "extensions" : []
  }
 ],
 [
  "smt_cap_reveal",
  {
   "control_account" : "delta",
   "cap" : { "amount" : 10000000, "nonce" : "0" },
   "extensions" : []
  }
 ],
 [
  "smt_cap_reveal",
  {
   "control_account" : "delta",
   "cap" : { "amount" : 10000000,  "nonce" : "0" },
   "extensions" : []
  }
 ]
]
```

#### Blocage des investissements

Il est possible de rendre indisponibles tout ou partie des investissements plutôt que des les transformer immédiatement en liquidités. Dans l’exemple suivant, 95 % sont bloqués.

```
"token_unit"           : [["$from.vesting", 95], ["$from", 5]]
```

#### Destruction du STEEM investi

Dans l’ICO suivante, le STEEM est détruit de manière irrévocable plutôt que d’aller dans le portefeuille d’un individu. Cette procédure imite la structure de l’ICO de Counterparty.

```
{
 "steem_unit" : [["null", 1]],
 "token_unit" : [["$from", 1]]
}
```

#### Blocage comme coût

Dans l’ICO suivante, il ne faut pas envoyer de STEEM au créateur du SMT en échange de tokens. Au lieu de cela, on bloque des STEEM (pour soi-même) et on reçoit un nombre de tokens correspondant aux STEEM bloqués.

```
{
 "steem_unit" : [["$from.vesting", 1]],
 "token_unit" : [["$from", 1]]
}
```

#### ICO hybrides & sans STEEM

Les ICO qui utilisent une autre monnaie que le STEEM pour leurs investissements, par exemple, SBD, BTC, ETH, etc., ne peuvent pas avoir lieu de manière totalement automatique sur la blockchain. Cependant, de telles ICO peuvent être contrôlées en transférant manuellement la répartition du montant de certains comptes fondateurs aux comptes STEEM des acheteurs proportionnellement à leurs investissements qui ne sont pas faits en STEEM.

### Paramètres d’inflation

La création de SMT après le lancement est appelée *inflation*.

L’inflation est le moyen par lequel les SMT récompensent les investisseurs pour la valeur qu’ils apportent.

Les épisodes inflationnistes suivent la structure suivante :

```
struct smt_inflation_unit
{
   flat_map< account_name_type, uint16_t >        token_unit;
};

// Event:  Support issuing tokens to target at time
struct token_inflation_event
{
   timestamp           schedule_time;
   smt_inflation_unit  unit;
   uint32_t            num_units;
};
```

Cet épisode affiche les unités `num_units` du token SMT.

#### Cible d’inflation possible

La cible est la personne qui est visée par l’inflation. La cible peut être un compte Steem normal, contrôlé par un individu, ou un compte sécurisé par multisignatures constitué de plusieurs créateurs.

De plus, plusieurs cibles spéciales sont possibles. Elles représentent des fonctions qui ne reposent pas sur la confiance et qui sont fournies par la blockchain elle-même :

- Récompenses. Une utilisation spéciale qui représente les récompenses de publication ou de vote.
- Investissement. Une utilisation spéciale qui représente les tokens qui garantissent les tokens investis.

#### Séquences d’événements

Traditionnellement, les blockchains calculent l’inflation bloc par bloc puisque les récompenses pour la production de blocs sont le principal (et souvent le seul) mécanisme d’inflation.

Cependant, il n’y a aucune bonne raison de coupler l’inflation à la production de blocs pour les SMT. En fait, les SMT ne donnent aucune récompense de bloc puisqu’ils n’ont pas de blocs (la fonction de production de blocs sur laquelle repose leur fonctionnement étant remplie par les témoins Steem, qui sont récompensés en STEEM).

Une répétition de l’inflation à intervalles réguliers peut être activée en ajoutant `interval_seconds` et `interval_count` à la structure de données de `token_inflation_event`. Le résultat est une nouvelle structure de données appelée `token_inflation_event_seq_v1`:

```
// Event seq v1:  Support repeatedly issuing tokens to target at time
struct token_inflation_event_seq_v1
{
   timestamp           schedule_time;
   smt_inflation_unit  unit;
   asset               new_smt;

   int32_t             interval_seconds;
   uint32_t            interval_count;
};
```

La structure de données représente un événement d’inflation de token qui se répète toutes les `interval_seconds` secondes, à `interval_count` reprises. La valeur entière maximale, `0xFFFFFFFF` est une valeur sentinelle spéciale qui représente une séquence d’événements se répétant sans fin.

Remarque: `new_smt` est une quantité de SMT, pas un nombre d’unités. Le nombre d’unités est déterminé en divisant `new_smt` par la somme des membres de unit.

#### Ajouter une inflation relative

La programmation de l’inflation est souvent exprimée par un pourcentage de l’offre plutôt que de manière absolue : 

```
// Event seq v2:  v1 + allow relative amount of tokens
struct token_inflation_event_seq_v2
{
   timestamp           schedule_time;
   smt_inflation_unit  unit;
   uint32_t            num_units;

   int32_t             interval_seconds;
   uint32_t            interval_count;

   asset               abs_amount;
   uint32_t            rel_amount_numerator;
};
```

Ensuite, nous calculons `new_smt` comme suit à partir de l’offre :

```
rel_amount = (smt_supply * rel_amount_numerator) / SMT_REL_AMOUNT_DENOMINATOR;
new_smt = max( abs_amount, rel_amount );
```

Si la valeur que nous donnons à `SMT_REL_AMOUNT_DENOMINATOR` est une puissance de deux, la division peut être optimisée pour devenir une opération de décalage de bits. Pour obtenir une gamme plus variable à partir des bits, nous pouvons permettre un décalage variable :

```
// Event seq v3:  v2 + specify shift in struct
struct token_inflation_event_seq_v3
{
   timestamp           schedule_time;
   smt_inflation_unit  unit;

   int32_t             interval_seconds;
   uint32_t            interval_count;

   asset               abs_amount;
   uint32_t            rel_amount_numerator;
   uint8_t             rel_amount_denom_bits;
};
```

Le calcul devient alors :

```
rel_amount = (smt_supply * rel_amount_numerator) >> rel_amount_denom_bits;
new_smt = max( abs_amount, rel_amount );
```

Bien sûr, l’implémentation de ces calculs doit faire attention à prendre en compte un éventuel débordement dans la valeur intermédiaire `smt_supply * rel_amount_numerator`!

#### Ajouter une modulation de temps

La modulation du temps permet d’implémenter un taux d’inflation qui change continuellement au fil du temps selon une application linéaire par morceaux. Il suffit de préciser les extrémités de gauche et de droite d’un intervalle de temps, et de spécifier les montants absolus pour ces deux extrémités :

```
// Event seq v4:  v3 + modulation over time
struct token_inflation_event_seq_v4
{
   timestamp           schedule_time;
   smt_inflation_unit  unit;

   int32_t             interval_seconds;
   uint32_t            interval_count;

   timestamp           lep_time;
   timestamp           rep_time;

   asset               lep_abs_amount;
   asset               rep_abs_amount;
   uint32_t            lep_rel_amount_numerator;
   uint32_t            rep_rel_amount_numerator;

   uint8_t             rel_amount_denom_bits;
};
```

Quelques remarques à ce sujet :

- Seul le numérateur des montants relatifs est interpolé, le dénominateur est le même aux deux extrémités.
- Pour les périodes qui se situent en deçà de l’extrémité gauche de l’intervalle de temps, le montant à l’extrémité gauche de l’intervalle est utilisé.
- Pour les périodes qui se situent au-delà de l’extrémité droite de l’intervalle de temps, le montant à l’extrémité droite de l’intervalle est utilisé.

Le code ressemble à ce qui suit:

```
if( now <= lep_time )
{
   abs_amount = lep_abs_amount;
   rel_amount_numerator = lep_rel_amount_numerator;
}
else if( now >= rep_time )
{
   abs_amount = rep_abs_amount;
   rel_amount_numerator = rep_rel_amount_numerator;
}
else
{
   // t is a number between 0.0 and 1.0
   // this calculation will need to be implemented
   // slightly re-arranged so it uses all integer math

   t = (now - lep_time) / (rep_time - lep_time)
   abs_amount = lep_abs_amount * (1-t) + rep_abs_amount * t;
   rel_amount_numerator = lep_rel_amount_numerator * (1-t) + rep_rel_amount_numerator * t;
}
```

#### Opérations inflationnistes

L’opération inflationniste est précisée comme suit :

```
struct smt_setup_inflation_operation
{
   account_name_type   control_account;

   timestamp           schedule_time;
   smt_inflation_unit  inflation_unit;

   int32_t             interval_seconds = 0;
   uint32_t            interval_count = 0;

   timestamp           lep_time;
   timestamp           rep_time;

   asset               lep_abs_amount;
   asset               rep_abs_amount;
   uint32_t            lep_rel_amount_numerator = 0;
   uint32_t            rep_rel_amount_numerator = 0;

   uint8_t             rel_amount_denom_bits = 0;

   extensions_type     extensions
};
```

L’opération `setup_inflation_operation` est une opération de *préréglage* qui doit être exécutée *avant* la `smt_setup_operation`. Voir la section sur les opérations de préréglage. 

#### FAQ : inflation

- Q:  Est-ce que les structures de données d’inflation des SMT peuvent exprimer [la tendance inflationniste actuelle de Steem](https://github.com/steemit/steem/issues/551)?
- R:  Oui (sauf pour les erreurs d’arrondissement).
- Q:  Est-ce que les structures de données d’inflation des SMT récompensent les détenteurs de compte directement après x mois/années ?
- R:  Oui.
- Q:  Je n’en ai rien à faire de la modulation du temps. Est-ce que je peux désactiver cette fonctionnalité ?
- R:  Oui. Il suffit de définir `lep_abs_amount == rep_abs_amount` et
  `lep_rel_amount_numerator == rep_rel_amount_numerator` à la même valeur, et de définir `lep_time = rep_time` (toute valeur fera l’affaire).
- Q:  Est-il possible de masquer une partie de ce qui est trop complexe grâce à une interface utilisateur bien conçue ?
- R:  Oui.
- Q:  Peut-on calculer l’inflation en fonction du temps avec exactitude ?
- R:  Les structures de données d’inflation peuvent être totalement modélisées/simulées. Pour certaines structures d’émission, les quantités émises dépendent des fonds levés, les structures d’émission ne peuvent alors être calculées avec exactitude.

### Paramètres de tokens nommés

Certains des comportements du STEEM sont influencés par des constantes de configuration définies au moment de la compilation qui sont implémentées via des instructions `#define` dans le code source C++ de `steemd`. Il est logique que des comportements équivalents pour les SMT soient configurables par le créateur de SMT.

Ces paramètres sont `runtime_parameters` et `setup_parameters`. Les
`setup_parameters` sont un champ dans `smt_setup_operation`; ils doivent être définis avant `smt_setup_operation`, et ne peuvent être modifiés après l’exécution de `smt_setup_operation`. Les `runtime_parameters` sont un champ de `smt_set_runtime_parameters_operation`, et ils peuvent être modifiés par le créateur du token à tout moment.

Ces opérations sont définies de la manière suivante :

```
struct smt_set_setup_parameters_operation
{
   account_name_type                                 control_account;

   flat_set< smt_setup_parameter >                   setup_parameters;
   extensions_type                                   extensions;
};

struct smt_set_runtime_parameters_operation
{
   account_name_type                                 control_account;

   flat_set< smt_runtime_parameter >                 runtime_parameters;
   extensions_type                                   extensions;
};
```

Actuellement, les paramètres `setup_parameters` et `runtime_parameters` suivants sont définis:

```
struct smt_param_allow_vesting                    { bool value = true;  };
struct smt_param_allow_voting                     { bool value = true;  };

typedef static_variant<
   smt_param_allow_vesting,
   smt_param_allow_voting
   > smt_setup_parameter;

struct smt_param_windows_v1
{
   uint32_t cashout_window_seconds = 0;              // STEEM_CASHOUT_WINDOW_SECONDS
   uint32_t reverse_auction_window_seconds = 0;      // STEEM_REVERSE_AUCTION_WINDOW_SECONDS
};

struct smt_param_vote_regeneration_period_seconds_v1
{
   uint32_t vote_regeneration_period_seconds = 0;    // STEEM_VOTE_REGENERATION_SECONDS
   uint32_t votes_per_regeneration_period = 0;
};

struct smt_param_rewards_v1
{
   uint128_t               content_constant = 0;
   uint16_t                percent_curation_rewards = 0;
   uint16_t                percent_content_rewards = 0;
   curve_id                author_reward_curve;
   curve_id                curation_reward_curve;
};

struct smt_param_allow_downvotes
{
   bool value = true;
};

typedef static_variant<
   smt_param_windows_v1,
   smt_param_vote_regeneration_period_seconds_v1,
   smt_param_rewards_v1,
   smt_param_allow_downvotes
   > smt_runtime_parameter;
```

Les interfaces utilisateur qui permettent d’inspecter ou de définir ces paramètres doivent prendre en compte le type et l’échelle de chaque paramètre. Les paramètres de pourcentage, en particulier, sont sur une échelle exprimée en point de base (dans laquelle 100 % correspond à une valeur de `STEEM_100_PERCENT = 10000`), et les interfaces ou autres outils de création ou d’inspection des transactions *doivent* utiliser cette échelle en point de base.

## Contraintes de paramétrage

De nombreux paramètres dynamiques doivent être limités pour empêcher les abus qui pourraient nuire aux utilisateurs de tokens.

- `0 < vote_regeneration_seconds < SMT_VESTING_WITHDRAW_INTERVAL_SECONDS`
- `0 <= reverse_auction_window_seconds + SMT_UPVOTE_LOCKOUT <
  cashout_window_seconds < SMT_VESTING_WITHDRAW_INTERVAL_SECONDS`

## Sémantiques d’investissement des SMT

Les SMT ont des sémantiques d’investissement similaires aux STEEM (Power up/Power down). En particulier :

- Les SMT peuvent faire l’objet d’un "Power up" vers un compte de blocage.
- Les SMT qui se trouvent sur le compte de blocage peuvent faire l’objet d’un "Power down" sur une période de 13 semaines (contrôlé par des paramètres statiques  `SMT_VESTING_WITHDRAW_INTERVALS`,
  `SMT_VESTING_WITHDRAW_INTERVAL_SECONDS`).
- Le vote n’est influencé que par les tokens qui ont subi un "Power up".
- Le solde du compte de blocage ne peut pas être transféré ni vendu. 

De plus, il est possible qu’une partie de l’inflation des tokens soit transférée vers des comptes de blocage. Ces tokens nouvellement émis sont divisés entre tous les utilisateurs qui possèdent des comptes de blocage, proportionnellement au nombre de tokens qu’ils ont investis. Comme le nombre de tokens émis ne dépend pas des comptes de blocage des utilisateurs, le taux de rendement que cela représente varie en fonction du nombre de tokens investis à la fois.

## Récompenses liées au contenu

Les tokens créés lors des émissions de SMT vont dans la réserve de récompenses. La blockchain utilise des algorithmes pour déterminer :

- (1) Comment répartir les récompenses au niveau du token entre les publications.
- (2) Comment répartir les récompenses d’une publication entre l’auteur et les curateurs (les upvoteurs) de la publication.

Les algorithmes qui résolvent ces problèmes fonctionnent de la manière suivante :

- (1) Les publications sont évaluées les unes par rapport aux autres en fonction de la *courbe des récompenses* ( ou `rc`).
- (2a) Les curateurs reçoivent collectivement un pourcentage fixe des récompenses de la publication, spécifié par le paramètre `curation_pct`.
- (2b) L’auteur reçoit le reste (après avoir pris en compte les récompenses dues à des bénéficiaires éventuels ou une limitation/un refus des récompenses par l’auteur).
- (2c) Les curateurs de la publication sont évalués les uns par rapport aux autres en fonction de la *courbe de curation* (ou `cc`).

![Creation](img/creation.png)
\begin{center}Figure 7: flux des tokens initiaux et des émissions de SMT\end{center}

## Courbes : notions

La courbe des récompenses peut être *linéaire* ou *quadratique*. La courbe des récompenses linéaire
`rc(r) = r` est indépendante des upvotes. La courbe des récompenses quadratique `rc(r) = r^2 + 2rs` a une pente croissante.

Pour comprendre à quoi servent les courbes des récompenses, il faut imaginer que l’on regroupe les publications qui ont récolté le plus d’upvotes de la manière suivante :

- La section A rassemble le top 10 % des publications par upvotes.
- La section B rassemble les 10 % suivants des publications par upvotes.

Les récompenses peuvent varier de la manière suivante :

- Dans les deux courbes des récompenses, les publications de la section A obtiendront de plus grandes récompenses que les publications de la section B, vu qu’elles ont obtenu plus d’upvotes.
- Dans la courbe des récompenses quadratique, les publications de la section A obtiendront un *coup de pouce* supplémentaire par rapport aux publications de la section B, étant donné que les publications de la section A recevront *plus de récompenses par upvote*.
- Dans la courbe des récompenses linéaire, la section A et la section B recevront les mêmes récompenses par upvote.

Les courbes de curation possibles sont :

- Linéaire, `cc(r) = r`
- Racine carrée, `cc(r) = sqrt(r)`
- Délimitée, `cc(r) = r / (r + 2s)`

Pour mieux visualiser, voici quelques graphiques. Chaque zone colorée représente la manière dont les récompenses de curation sont divisées entre des curateurs qui ont la même puissance de vote.

![Reward curves and curation curves](img/rc-cc.png)
\begin{center}Figure 8: Courbes des récompenses et courbes de curation\end{center}

- La colonne verticale rectangulaire montre la récompense immédiate reçue lors d’un upvote.
- La zone colorée qui s’étend vers la droite montre la façon dont les récompenses d’un curateur augmentent à mesure que d’autres curateurs upvotent après lui.
- Quand les deux courbes sont linéaires, chacun reçoit la même récompense de curation, quel que soit l’article pour lequel il vote.
- Dans le cas de `rc_linear + cc_sqrt` et de `rc_quadratic + cc_bounded`, les rectangles de même hauteur signifient que tout le monde reçoit une récompense de curation initiale plus ou moins identique. Appelons cela `ICR=`.
- Dans le cas de `rc_linear + cc_bounded`, la hauteur des rectangles diminue. Cela représente un *handicap* progressif au vote pour les publications déjà populaires. Appelons cela `ICR-`.
- Dans le cas de `rc_quadratic + cc_sqrt` et `rc_quadratic + cc_linear`, la hauteur des rectangles augmente. Appelons cela `ICR+`.

Fondamentalement, la curation consiste à prévoir que des upvotes auront lieu à l’avenir. En tant que concepteurs de systèmes de récompenses, notre critère pour sélectionner une courbe devrait être de récompenser les prévisions correctes. La courbe qui répond le mieux à ce critère dépend de la relation entre les upvotes actuels et futurs.

- Si les futurs upvotes d’une publication sont *indépendants* de ses upvotes actuels, une courbe `ICR=` est la plus adaptée.
- Si les futurs upvotes d’une publication sont *corrélés positivement* avec ses upvotes actuels, il vaut mieux choisir une courbe `ICR-`, idéalement ajustée au degré de corrélation.
- Si les futurs upvotes d’une publication sont *corrélés négativement* avec ses upvotes actuels, il vaut mieux choisir une courbe `ICR+`, idéalement ajustée au degré de corrélation.

En pratique, une situation d’indépendance ou de légère corrélation positive est la plus probable, il vaut donc mieux opter pour une courbe `ICR=` ou `ICR-`. Pour ce qui est de STEEM, à l’origine la curation correspondait à l’`ICR=`quadratique. Depuis le hard fork 19, elle correspond à l’`ICR=` linéaire.

## Objectif de vote par jour

Chaque compte possède du `voting_power`, qui repose sur le même principe que la barre de points de pouvoir dans les jeux vidéos et qui se régénère de 0 % à 100 % au fil du temps à un taux constant. Ce taux est déterminé par deux paramètres :  

- (a) Le temps qu’il faut pour régénérer cette barre à 100 %, `vote_regeneration_period_seconds`.
- (b) Le `voting_power` utilisé par un vote à 100 %.

Le `vote_regeneration_period_seconds` est précisé directement. Pour (b), au lieu de préciser directement la puissance de vote d’un vote à 100 %, il faut préciser `votes_per_regeneration_period`. Les votes à 100 % sont alors définis de sorte qu’un utilisateur qui effectue un nombre de votes à 100 % égal à `votes_per_regeneration_period` neutralise la régénération de la puissance de vote.

## Aperçu de l’interface graphique de création de SMT
![SMT configuration](img/SMT-setup.png)
\begin{center}Figure 9: Configuration des SMT\end{center}

## Potentiel de vote et de récompense

Cette section présente les concepts du *potentiel de vote* et du *potentiel de récompense*.

- Un token peut servir à *voter* pour un commentaire si ce token est fait pour avoir une influence sur le commentaire.
- Pour un vote donné, chaque token qui a servi à voter pour un commentaire est soit "rémunérateur" soit "consultatif".
- Si un token est rémunérateur, le vote influence les récompenses pour le commentaire.
- Si un token est consultatif, le vote n’influence pas les récompenses pour le commentaire.

Les votes consultatifs n’ont pas d’influence sur les récompenses ou sur la puissance de vote. Toutefois, les votes consultatifs sont tout de même appliqués par les algorithmes de classification et les calculs d’estimation des récompenses. Les interfaces utilisateur peuvent donc afficher des publications consultatives.

L’ensemble des tokens qui peuvent servir à voter est déterminé par `allowed_vote_assets` qui est une extension comment_options_extension.

```
struct allowed_vote_assets
{
   flat_map< asset_symbol_type, votable_asset_info >      votable_assets;
};

struct votable_asset_info_v1
{
   share_type        max_accepted_payout    = 0;
   bool              allow_curation_rewards = false;
};

typedef static_variant< votable_asset_info_v1 >           votable_asset_info;
```

Les règles suivantes sont d’application pour déterminer si les tokens peuvent servir à voter :

- Les STEEM peuvent servir à voter pour toutes les publications.
- Un token peut servir à voter pour une publication s’il apparaît dans les `votable_assets` de la publication.
- Dans le cas contraire, le token ne peut pas servir à voter pour cette publication.

Les règles suivantes permettent de déterminer si un token est rémunérateur :

- Pour pouvoir récompenser une publication, un token doit pouvoir servir à voter pour cette publication.
- Si, pour des tokens/publications, le `max_accepted_payout` du token de cette publication est zéro, le token ne peut pas servir à récompenser cette publication.
- Si une personne vote (upvote/downvote), mais que son token a une valeur nulle, ce token ne permettra pas au vote de cette personne d’être rémunérateur.
- Si le `max_accepted_payout` de n’importe quel token qui ne repose pas sur le STEEM est différent de zéro, le `max_accepted_payout` des STEEM/SBD doit alors être d’au moins le `max_accepted_payout` par défaut.

Remarques sur la mise en application :

- Pour un vote consultatif, toutes les récompenses sont nulles, y compris celles des curateurs et des bénéficiaires. Pourquoi ? Parce que la blockchain applique le plafond `max_accepted_payout` avant les calculs des curateurs et des bénéficiaires.
- Actuellement (depuis le 19e hard fork de Steem), la blockchain Steem déduit de la puissance de vote pour les votes consultatifs sur Steem. Ce comportement sera modifié dans un prochain hard fork de Steem (Steem numéro #1380).
- Deux tokens au maximum peuvent être précisés dans `votable_assets`. Cela veut dire que chaque publication est votée avec un maximum de trois tokens (y compris le STEEM)
- Le `max_accepted_payout` par défaut est enregistré dans `max_accepted_steem_payout_latch` qui fait partie de `dynamic_global_properties_object`.  Les clients doivent remplir le `max_accepted_payout` d’une publication en fonction de `max_accepted_steem_payout_latch` au cas où la valeur par défaut change dans une prochaine version.

Il n’existe pas de restriction au niveau du consensus qui oblige une publication à avoir des `allowed_vote_assets`précis. Ces publications peuvent alors signaler qu’elles acceptent les récompenses sous forme de n’importe quel token. Toutefois, les interfaces utilisateur peuvent imposer leurs propres règles de validation non consensuelles sur `allowed_vote_assets` et masquer les publications qui ne respectent pas ces règles de validation non consensuelles.

Par exemple, dans une communauté Hivemind qui possède un token correspondant, il peut y avoir une règle de validation qui veut que les `allowed_vote_assets` définis dans chaque publication au sein de cette communauté comprennent le token de cette communauté. C’est une règle de validation non consensuelle vu que le principe même d’une publication existant dans une communauté Hivemind est un principe non consensuel. Comme il s’agit d’une règle de validation non consensuelle, aucune logique consensuelle ne peut l’appliquer. Toutefois, les interfaces utilisateur qui connaissent les communautés Hivemind peuvent refuser de répertorier ou d’afficher les publications qui ne respectent pas cette règle de validation.

## Paramètres statiques des tokens

Les paramètres statiques sont des constantes de configuration qui affectent le comportement des SMT, mais sont délibérément exclues des `smt_setup_parameters` ou `smt_runtime_parameters`. La raison pour laquelle ils ne sont pas configurables est que permettre à ces paramètres de dévier de manière significative des valeurs utilisées pour le STEEM entraînerait des risques non négligeables, dont voici quelques exemples :

- L’implémentation pourrait être très compliquée.
- Les utilisateurs finaux pourraient être extrêmement contrariés.
- La sécurité et la stabilité du token pourraient être compromises.
- La sécurité et la stabilité du STEEM pourraient être compromises.

Voici la liste de ces paramètres statiques :

- `SMT_UPVOTE_LOCKOUT_HF17` : statique - Cette valeur désactive les upvotes un certain temps avant le paiement, pour empêcher une utilisation abusive des downvotes juste avant le paiement.
- `SMT_VESTING_WITHDRAW_INTERVALS` : statique
- `SMT_VESTING_WITHDRAW_INTERVAL_SECONDS` : statique
- `SMT_MAX_WITHDRAW_ROUTES` : statique
- `SMT_SAVINGS_WITHDRAW_TIME` : statique
- `SMT_SAVINGS_WITHDRAW_REQUEST_LIMIT` : statique
- `SMT_MAX_VOTE_CHANGES` : statique
- `SMT_MIN_VOTE_INTERVAL_SEC` : statique
- `SMT_MIN_ROOT_COMMENT_INTERVAL` : statique
- `SMT_MIN_REPLY_INTERVAL` : statique
- `SMT_MAX_COMMENT_DEPTH` : statique
- `SMT_SOFT_MAX_COMMENT_DEPTH` : statique
- `SMT_MIN_PERMLINK_LENGTH` : statique
- `SMT_MAX_PERMLINK_LENGTH` : statique

## Paramètres obligatoires des tokens

Les paramètres de tokens définis par `smt_setup_parameters` ou
`smt_runtime_parameters` ont des valeurs par défaut. Quelques paramètres équivalents à STEEM sont spécifiés par des champs `smt_setup_operation`. Ce sont les paramètres qui n’ont pas de valeur par défaut et doivent donc être spécifiés pour chaque ressource.

- `SMT_MAX_SHARE_SUPPLY` : défini par `smt_setup_operation.max_supply`
- `SMT_BLOCKCHAIN_PRECISION` : défini par `pow(10, smt_setup_operation.decimal_places)`
- `SMT_BLOCKCHAIN_PRECISION_DIGITS` : défini par `smt_setup_operation.decimal_places`

## Interaction des SMT avec les opérations existantes

- `comment_payout_beneficiaries` : les
  `comment_payout_beneficiaries` existants ne redirigeront que les STEEM. À l’avenir, une fonctionnalité des
  `comment_payout_beneficiaries` qui permet la redirection des récompenses SMT pourrait être ajoutée.
- `comment_options` : `max_accepted_payout`, `allow_votes` affecte uniquement les STEEM, reportez-vous aux informations [ici](#votability-and-rewardability) pour restreindre le  `max_accepted_payout` pour les actifs. `allow_curation_rewards` affecte tous les tokens.
- `vote_operation` : tokens multiples disponibles dans les options de vote du commentaire.
- `transfer_operation` : prend en charge tous les SMT.
- Paiements via un tiers (Escrow): ne prennent pas en charge les SMT.
- `transfer_to_vesting_operation` : prend en charge tous les SMT qui permettent l’investissement.
- `withdraw_vesting_operation` : prend en charge tous les SMT qui permettent l’investissement.
- `set_withdraw_vesting_route_operation` : ne prend pas en charge les SMT.
- `account_witness_vote_operation` : les SMT n’affectent pas les votes pour les témoins.
- `account_witness_proxy_operation` : les SMT n’affectent pas les votes pour les témoins.
- `feed_publish_operation` : les flux ne peuvent pas être publiés pour les SMT.
- `convert_operation` : les SMT ne peuvent pas être convertis.
- Opérations d’ordres à cours limité : les ordres à cours limité sont tout à fait pris en charge par l’échange de SMT contre des STEEM.
- `transfer_to_savings_operation` : les SMT permettent l’épargne.
- `decline_voting_rights_operation` : affecte les votes en SMT ainsi que les votes en STEEM.
- `claim_reward_balance_operation` : les restrictions sur cette opération sont assouplies pour permettre de déposer n’importe quelle ressource dans n’importe lequel des trois champs, y compris des SMT.
- `delegate_vesting_shares_operation` : Multisignature native : la gestion des opérations SMT signées par de multiples signatures n’a rien de "spécial". Si vous avez configuré votre compte de manière à exiger une sécurité à multisignature, alors tout ce que votre compte signe devra être signé avec plusieurs signatures, comme vous l’avez spécifié. Cela inclut les opérations que votre compte effectue en tant que compte de contrôle gérant un SMT, et les opérations que votre compte effectue en tant qu’utilisateur détenteur de tokens SMT.

\newcommand{\steem}{\texttt{STEEM}}
\newcommand{\mytoken}{\texttt{MYTOKEN}}

# Teneurs de marché automatisés pour les SMT

Les teneurs de marché automatisés sont des contrats intelligents, largement inspirés du [protocole Bancor
[2]](https://about.bancor.network/static/bancor_protocol_whitepaper_en.pdf), qui peuvent être conçus lors de la configuration de l’ICO d’un SMT pour assurer des liquidités constantes à une communauté SMT. Pour plus de simplicité, les teneurs de marché automatisés dans Steem peuvent seulement faire des échanges de STEEM contre n’importe quel SMT, et inversement. 

## Configuration

### Définitions de base

Supposons que $s$ représente une quantité de STEEM, $t$ représente une quantité d’un certain token (SMT), et $p$ représente un prix. $pt$ est alors évalué en STEEM. Si MYTOKEN se vend à $p = 0.05$ STEEM / MYTOKEN alors $t = 120$ MYTOKEN a une valeur de $pt = (0.05\ \mbox{STEEM / MYTOKEN}) \cdot (120\ \mbox{MYTOKEN}) = 6\ \mbox{STEEM}$.

Si un teneur de marché (ou n’importe quel agent économique) a un "portefeuille" (inventaire) à deux actifs contenant des STEEM $s$ et des tokens $t$, et que le prix des tokens est $p$, alors nous pouvons mesurer la valeur $v$ de ce portefeuille en unités de STEEM : $v(p, s, t) = s + pt$.

Une stratégie courante de gestion du portefeuille est d’exiger que les STEEM soient une fraction constante $r$ of du portefeuille, c’est-à-dire que $s = r v(p, s, t)$ et $0 < r < 1$. Cette stratégie s’appelle le \textit{taux constant du portefeuille} (CPR policy), et l’équation $s = r v(p, s, t)$ est le \textit{taux invariable CPR}.

Une autre stratégie de gestion du portefeuille, abordée dans le livre blanc de Bancor, est appelée CRR pour \textit{constant reserve ratio}. le taux constant de réserve. Pour aborder le CRR, considérons $T$.  comme étant le nombre total de tokens existants. Le taux invariable CRR est alors défini comme $s = r v(p, 0, T-t)$.

### Remarques sur les conventions

Nous devons expliquer en quoi notre convention diffère du livre blanc de Bancor. Parfois, quand une utilisatrice, Alice, interagit avec le teneur de marché, elle retire des tokens de son compte pour recevoir des STEEM du compte du teneur de marché. Benoît, quant à lui, peut ajouter des tokens à son compte en envoyant des STEEM au compte du teneur de marché. 

Bancor a pour convention que dans le cas présent, le teneur de marché *détruit* les tokens lors de son interaction avec Alice et *crée* des tokens lors de son interaction avec Benoît. La convention de Bancor suggère que le teneur de marché n’est pas un acteur ordinaire, mais a besoin de "pouvoirs spéciaux" accordés par le système (plus précisément, le monopole de l’émission des tokens) pour fonctionner.

Dans ce livre, nous adoptons une convention en vertu de laquelle les tokens envoyés par Alice au teneur de marché ne sont pas détruits, mais sont ajoutés à l’inventaire (le compte) du teneur de marché. De la même manière, les tokens envoyés à Benoît par le teneur de marché ne sont pas créés à partir de rien : ils existent déjà et sont simplement transférés de l’inventaire du teneur de marché à Benoît. Dès lors, nous pouvons voir que pour l’essentiel, le teneur de marché est un agent économique ordinaire qui se comporte conformément à un algorithme déterministe - il n’a pas besoin de "pouvoirs spéciaux" !

## Échanges finis

### Définitions de base

Un \textit{échange} est un changement de $(s, t) \to (s+\Delta s, t+\Delta t)$ dans le compte du teneur de marché. Le \textit{prix} auquel l’échange a lieu est défini comme $p = {- \Delta s \over \Delta t}$.  Nous nous limitons aux \textit{échanges se déroulant correctement} dans lesquels soit $\Delta s = \Delta t = 0$,
soit $\Delta s$ et $\Delta t$ ne sont pas égaux à 0 et sont de signe opposé.

Théorème : un échange effectué à un prix $p$ conserve sa valeur au prix $p$.  Plus rigoureusement, si $\Delta s, \Delta t$ représente un échange au prix $p$, alors $v(p, s, t) = v(p, s + \Delta s, t + \Delta t)$.

Définissons plus rigoureusement l'\textit{état} du teneur de marché comme un tuple $M = (s, t, T, r)$. Pour un prix $p$ donné, nous pouvons définir \textit{l’échange de restitution} à $p$ (aussi appelé \textit{échange de relaxation} ou a \textit{relaxation}) comme un échange qui a lieu au prix $p$ et a pour résultat un état qui respecte le taux invariable CRR.

### Calcul de l’échange de restitution

L’échange de restitution consiste en deux fonctions, $\Delta s(M, p)$ et $\Delta t(M, p)$. Nous pouvons calculer ces fonctions à partir de la définition du prix et du taux invariable CRR :

\begin{eqnarray*}
\Delta s & = & -p \Delta t \\
s + \Delta s & = & r v(p, 0, T-(t+\Delta t)) \\
\Rightarrow s - p \Delta t & = & r v(p, 0, T-t-\Delta t) \\
   & = & r p(T-t-\Delta t) \\
   & = & rpT - rpt - rp \Delta t \\
\Rightarrow r p \Delta t - p \Delta t & = & r p (T-t) - s \\
\Rightarrow \Delta t & = & {r p (T - t) - s \over rp - p } \\
      & = & \left( {1 \over 1-r} \right) \left( {s \over p} - r (T-t) \right) \\
\Rightarrow \Delta s & = & - p \Delta t \\
   & = & \left( {1 \over 1-r} \right) \left( r p (T - t) - s \right)
\end{eqnarray*}

### Computing the Equilibrium Price

Pour une situation $M$ donnée, il existe un prix $p_{eq}(M)$ pour lequel la valeur de l’échange de restitution est de zéro. On appelle ce prix le \textit{prix d’équilibre}.  Il est possible de calculer le prix d’équilibre en définissant $\Delta s = 0$:

\begin{eqnarray*}
\Delta s & = & 0 \\
& = & \left( {1 \over 1-r} \right) \left( r p_{eq} (T - t) - s \right) \\
\Rightarrow r p_{eq} (T - t) - s & = & 0 \\
\Rightarrow r p_{eq} (T - t) & = & s \\
\Rightarrow p_{eq} & = & {s \over r (T-t)}
\end{eqnarray*}

Théorème :  la restitution est idempotente. Cela veut dire qu’après une restitution à un prix $p$,
le prix d’équilibre de la situation obtenue est $p$, et la deuxième restitution au prix $p$ aura une valeur nulle.

### Exemple

Exemple:  Supposons que $M = (1200, 3600, 12000, 0.25)$ et $p = 0.5$.  Alors, sur les $T = 12000$ TOKEN existants, $t = 3600$ TOKEN sont détenus par le teneur de marché, donc $T-t = 12000 - 3600 = 8400$.

Les  TOKEN "circulent" (c’est-à-dire qu’ils existent dans des comptes en dehors du teneur de marché). Ces tokens en circulation valent $p(T-t) = 4200$ STEEM au total. Ils "devraient" donc être garantis par un niveau de réserve cible de $rp(T-t) = 4200 * 0.25 = 1050$ STEEM.

Dans cet exemple, il y a "trop" de STEEM dans la réserve, la restitution achètera donc des tokens sur le marché. Ce qui aura deux effets : cela fera diminuer la réserve de STEEM, et le nombre de tokens en circulation. La diminution du nombre de tokens en circulation, à son tour, entraîne la diminution du niveau de réserve cible. Pour chaque STEEM utilisé pour acheter des tokens, le niveau de réserve cible diminue de $r$ STEEM;
Vu que $r < 1$ , la réserve en diminution finira par "rattraper" son niveau cible, qui diminue plus lentement.

Le calcul ci-dessus montre que nous effectuerons ce rattrapage à $\Delta s = \left( {1 \over 1-r} \right) \left( r p (T - t) - s \right)$ et $\Delta t = \left( {1 \over 1-r} \right) \left( {s \over p} - r (T - t) \right)$.
En effectuant les calculs avec les nombres définis dans cet exemple, on a $\Delta s = -200$ STEEM and $\Delta t = 400$ TOKEN.

Vérifions (a) que ces valeurs calculées $\Delta s = -200, \Delta t = 400$
représentent un échange avec un prix de 0,5, et (b) que le taux invariable CRR s’applique à un nouvel état $M_{new} = (s+\Delta s, t+\Delta t, T, r)$.  En calculant $p = {- \Delta s \over \Delta t}$ nous obtenons effectivement $p = 0.5$.  Après l’exécution de cet échange, le teneur de marché a $s_{new} = s + \Delta s = 1200 - 200 = 1000$ STEEM, et $t_{new} = t + \Delta t = 3600 + 400 = 4000$ tokens.

Pour vérifier la condition (b) selon laquelle le taux invariable CRR s’applique toujours, nous répétons l’analyse dans le premier paragraphe de cet exemple avec les nouveaux nombres. Nous savons que $M_{new} = (1000, 4000, 12000, 0.25)$ et $p = 0.5$.  Donc, de $T = 12000$ TOKEN existants, $t_{new} = 4000$ TOKEN sont désormais détenus par le teneur de marché, donc $T-t_{new} = 12000 - 4000 = 8000$ TOKEN circulent. Ces tokens en circulation valent
$p(T-t_{new}) = 4000$ STEEM au total, Ils "devraient" donc être garantis par un niveau de réserve cible $rp(T-t) = 4000 * 0.25 = 1000$ STEEM.  Comme le niveau de réserve cible correspond en effet exactement au niveau de réserve réel $s_{new} = 1000$ STEEM, nous pouvons conclure que le taux invariable CRR est respecté après cet échange de restitution. 

## Échanges infinitésimaux

Cette section est assez technique. Une bonne compréhension du calcul et des équations différentielles sera nécessaire au lecteur pour suivre les résultats.

### Mise en place du problème

Supposons que nous remplissons la condition d’invariabilité à un prix $p = p_{eq}$; via un taux invariable CRR $s = r v( p, 0, T-t) = r p (T-t)$.
Supposons que le prix augmente pour atteindre $p + \Delta p$ et qu’un échange de restitution $\Delta s, \Delta t$ a lieu à ce nouveau prix.

Dans cette section, nous envisageons une situation limitée dans laquelle $\Delta p$ est extrêmement petit, nous utiliserons donc la notation de Leibniz ($dp$ pour un petit changement de $p$, $ds$ pour un petit changement de $s$, $dt$ pour un petit changement de $t$).

### Résolution des équations différentielles

En appliquant la substitution $p \gets p + dp$ à l’expression de ∆s calculée dans la section précédente, nous obtenons une expression qui se simplifie en une équation différentielle séparable qui peut être résolue :

\begin{eqnarray*}
ds & = & {1 \over 1-r} \left( r (p + dp) (T - t) - s \right) \\
   & = & {1 \over 1-r} \left( r p (T - t) + r dp (T - t) - r p (T - t) \right) \\
   & = & {1 \over 1-r} r (T - t) dp \\
   & = & {1 \over 1-r} \left( {s \over p} \right) dp \\
\Rightarrow {1 \over p} dp & = & (1-r) \left( {1 \over s} ds \right) \\
\Rightarrow \int {1 \over p} dp & = & (1-r) \int {1 \over s} ds \\
\Rightarrow \ln(p) & = & (1-r) \ln(s) + C_0 \\
\Rightarrow p & = & k_0 s^{1-r}
\end{eqnarray*}

De la même manière, pour $t$, nous pouvons partir de $dt = -ds / p$ et obtenir et résoudre une équation différentielle à variable séparable :

\begin{eqnarray*}
dt & = & -ds / p \\
   & = & -{r \over 1-r} (T - t) dp / p \\
\Rightarrow {1 \over T-t} dt & = & -{r \over 1-r} \left( {1 \over p} \right) dp \\
\Rightarrow {1 \over p} dp & = & {1-r \over r} \left( {1 \over t-T} \right) dt \\
\Rightarrow \int {1 \over p} dp & = & {1-r \over r} \int {1 \over t-T} dt \\
\Rightarrow \ln(p) & = & {1-r \over r} \ln | t-T | + C_1 \\
\Rightarrow p & = & k_1 (T-t)^{1-r \over r}
\end{eqnarray*}

## Discussion qualitative 

Dans un teneur de marché CRR, par quoi les tokens nouvellement émis sont-ils "garantis" ?

L’une des options est de réduire le taux de réserve r. Cette option entraîne une absence d’activité immédiate sur le marché, mais affaiblit la réaction du teneur de marché à d’éventuelles futures modifications des prix. C’est ce qu’on appelle l’option "payer plus tard".

Une autre option est de modifier les conditions initiales du système dynamique, autrement dit de modifier les constantes d’intégration. Cette option entraîne une chute du prix d’équilibre $p_{eq}$ ce qui signifie que le teneur de marché va vendre les tokens à prix réduit pour renflouer la réserve. Si les carnets de commande sont bien remplis en comparaison avec le volume d’émission et qu’il y a suffisamment d’acheteurs pour les tokens, alors les ventes pourront renflouer la réserve et maintenir le prix d’équilibre à une valeur proche de son ancienne valeur. En effet, les carnets de commande bien remplis permettent de résister à la modification des prix entraînée par le teneur de marché. Si les carnets de commandes ne sont pas très remplis en comparaison avec le volume d’émission et qu’il y a peu ou pas d’acheteurs pour le token, alors le prix d’équilibre va chuter, épuiser le petit nombre des commandes et faire baisser le prix du marché. Puisque peu ou pas de tokens ont été vendus, même si la quantité *absolue* de STEEM dans la réserve est presque / exactement la même qu’avant, la valeur *relative* de la réserve par rapport à la capitalisation boursière amoindrie du token a augmenté jusqu’au taux de réserve. C’est l’option "payer maintenant".

## FAQ

Q:  Quel est le bien-fondé de la stratégie du taux constant de portefeuille ?

R:  Cette stratégie pourrait être rendue disponible pour les teneurs de marché à l’avenir.

Q:  Est-ce que le taux de réserve peut excéder les 100 % ? 

R:  Non.

Q:  Est-ce que le taux de réserve peut être égal à 100 % ?

R:  Pas avec le système décrit dans ce livre blanc. Il pourrait être possible de le coder en tant que cas particulier.

Q:  Dans le cas d’un teneur de marché CRR, d’où provient la "garantie" pour les tokens nouvellement émis ?

R:  En tant que créateurs de la blockchain, nous avons deux options pour assurer la "garantie". La première est de réduire le taux de réserve r. Cette option entraîne une absence d’activité immédiate sur le marché, mais affaiblit la réaction du teneur de marché à d’éventuelles futures modifications des prix. C’est ce qu’on appelle l’option "payer plus tard".

La deuxième option est de modifier les conditions initiales du système dynamique, autrement dit de modifier les constantes d’intégration. Cette option entraîne une chute du prix d’équilibre $p_{eq}$ ce qui signifie que le teneur de marché va vendre les tokens à prix réduit pour renflouer la réserve. Si les carnets de commandes sont bien remplis en comparaison avec la quantité d’émission et qu’il y a suffisamment d’acheteurs pour les tokens, alors les ventes pourront renflouer la réserve et maintenir le prix d’équilibre à une valeur proche de son ancienne valeur. En effet, les carnets de commandes bien remplis permettent de résister à la modification des prix entraînée par le teneur de marché. 

Si les carnets de commandes ne sont pas très remplis en comparaison avec le volume d’émission et qu’il y a peu ou pas d’acheteurs pour le token, alors le prix d’équilibre va chuter, épuiser le petit nombre des commandes et faire baisser le prix du marché. Puisque peu ou pas de tokens ont été vendus, même si la quantité *absolue* de STEEM dans la réserve est presque / exactement la même qu’avant, la valeur *relative* de la réserve par rapport à la capitalisation boursière amoindrie du token a augmenté jusqu’au taux de réserve. C’est l’option "payer maintenant".

Q:  Où est l’option « ne pas payer » ?

R:  Vous devez trouver comment il est possible de "garantir" les tokens nouvellement émis. À moins qu’il n’y ait pas d’émission, ni de « garantie » pour aucun token. L’option "ne pas payer" serait donc un SMT soit sans émission, soit sans teneur de marché.

Q:  Est-ce que l’implémentation des exposants fractionnaires ne nécessite pas l’utilisation de virgules flottantes ?

R:  Seulement si vous avez besoin d’une précision relativement élevée (ce n’est pas notre cas), si vous n’accordez pas d’importance à la reproductibilité bit à bit dans les compilateurs, les systèmes d’exploitation, les processeurs, etc. (c’est notre cas) et si vous devez faire rapidement un très grand nombre de calculs (ce n’est pas notre cas). Une implémentation rapide, approximative et uniquement en nombres entiers est possible.

Q:  Est-ce que ce teneur de marché interagit avec le carnet de commandes à travers le système d’ordre à cours limité existant, ou sont-ce un ensemble d’opérations séparées ?

R:  En théorie, cela pourrait être implémenté dans les deux cas. Toutefois, il est plus probable que le teneur de marché soit implémenté en dehors des marchés de carnet de commandes pour que son code puisse être modifié. En pratique, s’il est implémenté comme étant un sous-système complètement isolé, des robots d’arbitrage seront mis en place pour éliminer toute différence de prix entre le système de réserve et le système de marché existant.

Q:  D’où viennent les quantités initiales de tokens des teneurs de marché ? 

R:  Les unités des ICO peuvent définir le teneur de marché comme étant un destinataire. Un créateur d’ICO peut déterminer qu’un pourcentage des investissements en STEEM dans l’ICO est destiné au teneur de marché. Il suffit de le définir, un peu comme on définit un fondateur. Le créateur d’ICO peut également se servir du système de plafond souple pour définir que tous les STEEM au-delà d’un montant prédéterminé sont destinés à l’ICO. Pareillement, un montant fixe ou un pourcentage des tokens peuvent être ajoutés dans l’ICO pour augmenter la quantité des tokens du teneur de marché.

Q:  Quelqu’un peut-il envoyer des STEEM ou des tokens au teneur de marché ?

R:  Oui.

Q:  Quels effets indésirables sont provoqués par l’envoi de STEEM ou de tokens au teneur de marché ?

R:  Les constantes d’intégration sont réinitialisées, ce qui veut dire que le prix d’équilibre va être modifié. Le teneur de marché va vendre les actifs à prix réduit. 

Q:  Cela ne va-t-il pas engendrer de la manipulation ou l’appropriation de l’inventaire du teneur de marché pour faire du profit privé ?

R:  Envoyer des actifs au teneur de marché a pour effet qu’il va se lancer dans des activités d’échange, ce qui aura une influence sur le prix. Toutefois, en déversant un montant identique sur le marché, il y aura une plus grande activité commerciale et un effet plus important sur le prix. Si Ève veut dépenser ses tokens/STEEM pour manipuler les prix, elle préférera une stratégie consistant à simplement déverser des tokens/STEEM sur le marché, vu que cette stratégie est plus rentable pour elle.

Q:  Est-ce que l’activité des teneurs de marché génère des bénéfices (pertes) ?

R:  Cela dépend de comment on mesure les « bénéfices ». Si la valeur des STEEM et des tokens est mesurée grâce à une devise tierce externe telle que le dollar américain ou le bitcoin, l’inventaire du teneur de marché, estimé en cette devise, peut évidemment augmenter ou diminuer de valeur. Si les gens envoient des STEEM ou des TOKENS volontairement au teneur de marché, cette activité augmente évidemment la valeur du teneur de marché, qu’importe l’unité de mesure utilisée.

Une autre façon de définir les bénéfices est d’utiliser les constantes d’intégration. Si les deux constantes d’intégration augmentent, ou si l’une augmente et l’autre reste inchangée, on constate une augmentation minime pour chaque échange quand le teneur de marché est en mode "preneur".

Q:  Qu’est-ce que le mode "preneur" ? Comment configurer un teneur de marché pour qu’il fonctionne en mode "preneur" ?

R:  Quand les commandes sont exécutées, la commande utilisée pour fixer le prix est appelée "faiseur". La contrepartie du faiseur est le preneur. Sur le marché du STEEM sur la blockchain (et sur presque toutes les plateformes d’échange), la commande plus ancienne est toujours le faiseur. 

Quand le teneur de marché est en mode preneur, ses actions sont toujours considérées comme des commandes preneur, qui sont exécutées au prix spécifié par l’utilisateur qui fait office de contrepartie (ce prix est toujours un peu plus avantageux que ce que le teneur de marché est prêt à accepter). Quand le teneur de marché n’est pas en mode preneur, ses actions sont toujours considérées comme étant des commandes faiseur. Cela ne crée pas de modifications dans les constantes d’intégration.

Le mode "preneur" est un paramètre d’exécution qui peut être programmé par le compte de contrôle des SMT.

Q:  Qui profite des bénéfices d’un teneur de marché en mode "preneur" ?

R:  Peut-être personne, ou peut-être tout le monde. C’est décentralisé.

Q:  OK, si mon SMT atteint un prix stable, le STEEM dans la réserve y restera normalement bloqué pour toujours. C’est pas très sympa. Comment programmer mon SMT pour que ce STEEM puisse être déverrouillé pour les bénéfices des utilisateurs de mon SMT ?

R:  Lors de la configuration, activez le paramètre "taux de réserve en déclin", ou DRR (decaying reserve ratio). Si vous activez le DRR, le taux de réserve chutera lentement jusqu’à atteindre une valeur prédéfinie, en utilisant l’excédent de STEEM dans les réserves pour acheter des tokens supplémentaires. Définir le DRR est un excellent moyen juste et décentralisé de rendre les capitalisations excédentaires aux investisseurs dans une ICO "plus populaire que prévu" qui engendre plus de fonds que ce que les sponsors peuvent dépenser.

Q:  Si le taux de réserve peut subir des modifications dues à des émissions "payez plus tard" ou à des DRR, est-ce vraiment un taux de réserve constant ?

R:  Non. On parle de taux de réserve "constant" parce qu’il est constant à court terme, dans des conditions normales ou dans les conditions de Bancor, qui lui a donné son nom. On peut dire que cette appellation est légèrement trompeuse.

Q:  Si les constantes d’intégration peuvent subir des modifications au fil du temps, peut-on vraiment dire qu’elles sont constantes ?

R:  Non. On les appelle constantes d’intégration parce que c’est leur rôle mathématique dans le calcul qui les présente. Elles porteront peut-être un nom différent dans une prochaine version de ce livre blanc.

Q:  Est-ce que je peux apporter une contribution de type "payer plus tard" à un DRR, de sorte que le taux de réserve *augmente* et que cette augmentation soit annulée plus tard par la diminution à venir ? Pourquoi devrais-je faire cela ?

R:  Oui. C’est un moyen de donner une contribution au teneur de marché, à la condition qu’il ne soit pas permis de se débarrasser immédiatement d’une partie de la contribution. C’est utile si vous voulez contribuer largement à un teneur de marché sans qu’il cause de perturbation en mettant une part importante de votre contribution sur le marché.

Q:  Est-ce que je peux stipuler qu’un DRR avec émission doit utiliser l’option "payez plus tard" pour les émissions quand le RR diminue ?

R:  Oui.

Q:  Est-ce que le teneur de marché dont il est question ici est équivalent à un échangeur de tokens Bancor ?

R:  Non. Un échangeur de tokens Bancor possède des taux de réserve multiples qui doivent atteindre 100 %, et requiert un troisième token qui représente une égalité sur l’échange de tokens. Le teneur de marché repris ici n’a aucune de ces caractéristiques.

Q:  Je veux profiter d’une période initiale de "découverte des prix" au cours de laquelle les gens font des échanges sans action du teneur de marché pour qu’ensuite, des tokens et des STEEM de l’ICO arrivent graduellement auprès du teneur de marché. Le teneur de marché connaît donc un démarrage lent après un certain délai, en partant de zéro jusqu’à avoir un pouvoir total. Est-ce possible ?

R:  On appelle cela la "propagation graduelle" et cette méthode peut être prise en charge.

Q:  Quid de la stabilité numérique ?

R:  Un teneur de marché ne peut intervenir que quand le solde de ses comptes dépasse un certain montant minimum pour chacun des deux actifs. De plus, les taux de réserve seront compris dans une certaine plage et tous les mécanismes qui définissent / diminuent / augmentent un taux de réserve seront contraints de faire en sorte que ces taux n’aillent pas au-delà des limites de cette plage. Des expériences numériques préliminaires indiquent que les limites devraient être de 10 000 satoshis pour les deux actifs, et de 5 % et 50 % respectivement pour les extrémités de la plage. Ces valeurs peuvent faire l’objet de modifications lors de prochains tests, expériences et analyses de scénarios catastrophes.

# Coût des opérations SMT et limitation de bande passante

Comme le STEEM, les SMT peuvent être transférés sur la blockchain Steem sans frais. Steem remplace les frais par une limitation de bande passante basée sur la quantité de STEEM qu’un utilisateur a investie. Autrement dit, la blockchain calcule la quantité de STEEM qu’un compte a temporairement bloquée pour déterminer la bande passante dont le compte dispose pour procéder à des transferts, publier et effectuer d’autres opérations au cours d’une période donnée. Dans une future version de Steem, [posséder un nom d’utilisateur pourrait donner accès à une petite quantité de bande passante pour permettre une expérience utilisateur encore meilleure.](https://steemit.com/steemit/@steemitblog/proposing-hardfork-0-20-0-velocity).

## Les opérations sans frais : indispensables pour une expérience utilisateur de qualité

Du fait de la limitation de la bande passante, il est probable que Steem ne réclamera jamais de frais de transaction aux utilisateurs ou aux applications pour des opérations de base comme le vote, la publication et le transfert de tokens. Cette absence de frais permet aux applications basées sur Steem d’être compétitives par rapport à leurs concurrentes qui ne sont pas basées sur la blockchain, comme Facebook ou Reddit, qui ne font évidemment pas payer de frais pour des actions comme ‘Like’ et ‘Upvote’. Si ces applications faisaient payer leurs utilisateurs, elles seraient moins utilisées.

# Échange décentralisé

L’une des fonctionnalités utiles des SMT est leur accès immédiat à des marchés automatisés fonctionnels reposant sur un actif liquide, le STEEM.

## Mise en relation automatique des commandes

Les structures d’échange décentralisé (decentralized exchange ou DEX) de Steem permettent aux actifs d’être automatiquement mis en relation pour obtenir le meilleur prix quand les offres et les demandes se rencontrent, contrairement aux autres DEX, qui nécessitent un « intermédiaire » ou un agent utilisateur pour mettre les commandes en relation. Une mise en relation des commandes automatisée plutôt que facilitée par un intermédiaire est importante pour la sécurité des actifs basés sur Steem et pour la reproductibilité et la sécurité des interfaces DEX.

## Types d’actifs divers

Les utilisateurs et créateurs de SMT auront accès à plusieurs actifs via le DEX de Steem : le STEEM, les SBD, les SMT, et les dérivés simples (reconnaissances de dettes). Ces actifs voisins peuvent améliorer la visibilité et l’effet de réseau de tous les SMT créés.

Le STEEM est le token donnant accès aux actifs émis sur Steem, et il est utile, car il sert d’outil de mesure de la bande passante pour tous les SMT de Steem. Le STEEM est également la ressource utilisée par tous, qui sert de monnaie d’échange entre les SMT.

Les SBD (Steem Blockchain Dollars) sont un actif expérimental sur Steem et sont liés au dollar américain. Ils sont apparus au lancement de Steem en 2016. Il n’est pas sûr que les SBD apporteront une valeur ajoutée aux détenteurs de dollars comme ils seront soumis à la concurrence des tokens de reconnaissance de dette en dollars (qui pourrait les désavantager). Cependant, les SBD apporteront une valeur ajoutée aux spéculateurs.

Les SMT décrits dans cette proposition sont l’un des éléments nécessaires à la croissance de l’écosystème des tokens et à la généralisation de l’utilisation des actifs en cryptomonnaies. Les SMT seront échangés contre du STEEM via le DEX.

Les dérivés simples (reconnaissances de dettes) seront possibles via l’émission de SMT. Par exemple, si un SMT est émis sans propriétés d’inflation ni de réserve de récompenses, alors l’émetteur peut sans problème lier le prix du token à celui d’un autre actif réel comme le bitcoin ou le dollar. Dans ce cas, l’émetteur pourrait créer une entreprise servant de "porte d’entrée" en échangeant sa reconnaissance de dette contre du BTC ou des dollars. Les utilisateurs achèteraient la reconnaissance de dette pour avoir accès au DEX de Steem. Ce marché ajouterait de la diversité et un flux de valeurs à l’écosystème Steem tout en améliorant l’effet de réseau du DEX.

## Aucuns frais de transaction et de transfert

Le DEX de Steem est le premier DEX sans frais de transaction, ce qui profite autant aux créateurs de SMT qu’aux traders. Cela est rendu possible par [la limitation de la bande passante](#--fee--less-operations-necessary-for-quality-user-experience)
(décrite dans le livre blanc et dans le livre bleu de Steem), le processus selon lequel la blockchain calcule les "prix" des transactions octet par octet et détermine la bande passante dont dispose temporairement un compte pour effectuer des transactions. Ces "prix" relèvent de la comptabilité interne de la blockchain et ne représentent pas un coût en tokens.

# Ajout de fonctionnalités aux SMT au moyen de contrats natifs additionnels

Il existe plusieurs contrats programmables, potentiellement utiles, qui ne rentrent pas directement dans le cadre des SMT. Cependant, ces fonctionnalités des contrats peuvent être créées dans le cadre de projets modulaires ultérieurs qui permettent aux entrepreneurs et aux communautés de faire croître les écosystèmes SMT de manière plus créative.

## Développement de communautés via des postes rémunérés

Les communautés liées aux SMT peuvent être stimulées par des postes rémunérés, des rôles dans des guildes, ou des métiers qui sont définis dans des contrats intelligents natifs et attribués à des participants élus continuellement. Les récompenses reçues en occupant un poste après avoir été élu sont issues d’une partie des allocations dont bénéficient les fondateurs du token, ou de dons qui sont envoyés à un contrat de poste rémunéré. Dans les contrats de poste rémunéré, il est possible de définir la durée de l’emploi, la fréquence et le volume des paiements, le token spécifique utilisé pour les élections pondérées par l’enjeu, le pourcentage du token nécessaire pour qu’un participant soit élu, et la manière dont les tokens dans les contrats de poste rémunéré sont redistribués ou abandonnés au cas où aucun participant n’est élu.

Les rôles rémunérés peuvent être utilisés pour faciliter le fonctionnement de nombreuses applications, jeux et entreprises basés sur un SMT. Un contrat de poste rémunéré, la programmation des récompenses du poste et les seuils de vote requis pour élire un compte à un poste rémunéré peuvent être créés par n’importe qui, moyennant des frais. Afin d’établir les tâches qui incombent à ces postes, des descriptions de poste ou des constitutions qui encouragent la conformité aux attentes en matière de performances peuvent être établies par l’émetteur ou la communauté du token. Il peut y avoir un nombre illimité de postes rémunérés, et les contrats de poste rémunéré peuvent recevoir n’importe quelle quantité des allocations de fondateur ou des dons de la communauté d’un token. Les types de postes rémunérés qui peuvent être employés vont du développeur front end à l’évangéliste en passant par le créateur de contenu éducatif et le représentant de commerce, ainsi que de nombreux autres rôles qui n’ont pas encore été inventés.

## Des SMT démocratiques grâce aux listes blanches d'oracles

Les SMT représentent un accès complètement ouvert aux tokens. Cependant, certaines entités voudront peut-être employer des algorithmes de limitation (un seul compte sur liste blanche, un seul vote par article et un quota de x votes par jour) pour augmenter le potentiel de leur token du point de vue de l’efficacité des mécanismes de découverte de contenu reposant sur la sagesse collective et rendre leur communauté plus démocratique. Pour rendre cette fonctionnalité possible, la réserve de récompenses d’un token devra être associée à une liste blanche gérable qui ne pourra être activée qu’au moment du lancement. La gestion de la liste blanche peut être prise en charge par l’entité qui lance le token ou déléguée à un service de gestion de l’identité comme Civic ou Jumio. Le service devra publier dans la blockchain Steem une liste des noms d’utilisateur Steem des gens connus/identifiés et la mettre périodiquement à jour pour que la liste blanche soit d’actualité. Quand la blockchain envoie des récompenses à un token, elle vérifie que le compte qui reçoit le token est dans la liste blanche, sans quoi les tokens sont remis dans la réserve de récompenses.

## ICO secondaires pour des levées de fonds multiples

Les entrepreneurs utilisant les SMT pour financer des projets pourraient avoir besoin d’effectuer des ventes aux enchères de tokens après le lancement initial du token. L’entrepreneur peut réserver des tokens de fondateur lors du lancement et les conserver pour les vendre plus tard. Cependant, il peut être préférable de vendre ces tokens aux enchères plutôt que dans des carnets de commandes « offre/demande » ou de gré à gré. Pour permettre des ICO secondaires de type vente aux enchères, un contrat secondaire de vente aux enchères doit être établi. Ce contrat nécessite de définir le début et la durée d’une ICO ainsi que des périodes de blocage des tokens achetés. La période de blocage permet de vendre des tokens à prix réduit sur les marchés ouverts et d’attirer un capital d’investissement qui resterait normalement hors du marché. L’entrepreneur enverra des tokens à ce contrat avant le début de la vente aux enchères et les tokens seront distribués aux participants de la vente immédiatement au terme de la période d’enchères.

## Partage de la bande passante avec les SMT sur base de leur réserve de liquidités

Les SMT qui utilisent des ICO pour créer des teneurs de marché automatisés afin d’augmenter la liquidité des tokens hériteront de droits sur la bande passante proportionnels à la quantité de STEEM présente dans la réserve du teneur de marché automatisé. Cet héritage de bande passante donne des droits de transaction de STEEM vers tous les SMT investis et ayant fait l’objet d’un « power up » et, pour simplifier, permet aux propriétaires de SMT d’effectuer des transactions proportionnellement à leur investissement en SMT sans posséder de STEEM à proprement parler. Le partage de bande passante basé sur les réserves de liquidités permet aux nouveaux tokens de fonctionner d’une manière encore plus indépendante tout en apportant de la valeur au STEEM de manière proportionnelle.

# Pourquoi les SMT sont-ils plus adaptés aux blockchains dont l’application est spécifique, comme Steem, plutôt qu’aux blockchains dont l’application est générale, comme Ethereum ?

À travers l’histoire du développement logiciel et matériel, il a été observé que les performances des systèmes spécialisés pourraient dépasser largement celles des systèmes à visée générale. Un exemple : [les cartes graphiques sont plus performantes que les processeurs](https://www.quora.com/Whats-the-difference-between-a-CPU-and-a-GPU-When-I-switch-on-my-computer-it-shows-GPU-information-What-does-it-mean)
grâce à leur spécialisation, et [les ASICS accomplissent certaines tâches mieux que les cartes graphiques](https://arstechnica.com/civis/viewtopic.php?t=1203755). Par conséquent, certains se demandent pourquoi une blockchain spécialisée telle que Steem, qui offre une programmabilité spécifique à une application et des mécanismes statiques reposant sur le consensus, est plus adaptée aux SMT que des blockchains d’application générale à programmabilité ouverte comme Ethereum, qui offre des contrats intelligents [Turing-complets](https://en.wikipedia.org/wiki/Turing_completeness)(programmables "à l’infini") dans une couche au-delà du consensus et a montré son utilité pour la découverte de nouveaux concepts dans le domaine des cryptomonnaies. Sans parler des avantages de Steem en termes d’effet de réseau et d’expérience des développeurs, les avantages de l’utilisation de Steem pour faire fonctionner les SMT sont visibles autant du point de vue informatique que du point de vue de la protection du consommateur et des perspectives économiques.

## Les SMT sont plus sûrs et plus économiques dans des environnements blockchain spécifiques à une application

La valeur des SMT dans un environnement natif de programmabilité spécialisée tel que Steem vient de la fiabilité du code et de l’efficacité découlant de cette fiabilité, alors que sur les plateformes d’application générale comme Ethereum et Tezos, les nouveaux tokens et leurs créateurs doivent faire l’objet d’un audit coûteux (et, dans une large mesure, basé sur des suppositions) pour vérifier qu’ils ne présentent aucun risque. Certains de ces protocoles à programmabilité générale déclarent disposer d’une [vérification formelle](https://en.wikipedia.org/wiki/Formal_verification), ce qui est utile. Cependant, la majorité du coût de l’audit subsiste étant donné que les mécanismes de fonctionnement du token que choisit l’émetteur, le choix du client utilisé pour écrire le code du token et la syntaxe de ce code doivent être soumis à des contrôles. Grâce à la conception ciblée de son code, Steem permet aux SMT d’avoir des propriétés cryptoéconomiques statiques (plutôt que dynamiques) qui peuvent être ajustées après le lancement d’un token sans que chaque modification ne soit une nuisance potentielle pour les détenteurs du token. La délimitation délibérée entre les propriétés économiques qui doivent être statiques et celles qui doivent être dynamiques facilite les audits nécessaires à la sécurité des tokens et les rend moins coûteux.

Pour illustrer ce problème, imaginons que quelqu’un vous offre 20 % de sa monnaie en échange de 100 $. Vous aurez des questions supplémentaires à poser au vendeur, principalement des questions visant à vérifier que l’affaire se déroule bien comme prévu, du genre « Le vendeur se réserve-t-il le droit d’imprimer plus de devises, et donc de diluer la valeur de mon achat ? » Les détenteurs de SMT, quant à eux, pourront être certains du fonctionnement économique de base des SMT qu’ils achètent grâce à la nature statique des propriétés économiques des SMT, telles que les taux d’émission et d’inflation, qui ne peuvent être modifiées par l’émetteur après le lancement. Dès lors, toute nouvelle émission inattendue de monnaie pouvant nuire au consommateur est impossible. Dans les protocoles blockchain à application générale et à programmabilité ouverte, comme Ethereum et Tezos, ce genre de mécanismes et de systèmes permettant d’assurer la fiabilité et la protection du consommateur à l’échelle de la plateforme ne pourraient pas exister.

## Les SMT sur Steem ont des incitants "Proof of Brain" alignés sur ceux du token de base

Contrairement au STEEM, les tokens de base (comme ETH) qui ne proposent pas de récompenses de contenu basées sur le Proof of Brain ne peuvent offrir la monétisation, une base d’utilisateurs active et avertie, le partage de l’influence et des bénéfices d’amorçage aux nouvelles communautés SMT. Le STEEM, en revanche, peut faire profiter de nouveaux réseaux des fonctionnalités de sa réserve de récompenses et de sa base d’utilisateurs avertis pour aider ces réseaux à démarrer, faire leur entrée sur le marché et former des groupes de participants indépendants et prospères sur le réseau. À l’inverse, certains entrepreneurs choisiront une stratégie visant à employer les SMT presque indépendamment du STEEM dans laquelle, comme les ERC20 sur Ethereum, les SMT peuvent fonctionner pendant que le STEEM tourne uniquement en arrière-plan et calcule la bande passante nécessaire pour les coûts de transaction.

## Les coûts de transaction des SMT sur Steem contribuent à une expérience utilisateur de qualité

Qu’elle soit basée sur la limitation de bande passante ou sur des frais de transaction au sens propre, aucune blockchain d’usage général ne peut attribuer de frais de transaction adéquats à plus d’une petite partie de ses applications, et l’expérience des utilisateurs des SMT (user experience ou UX) sur des blockchains à usage général (telles qu’Ethereum) en serait amoindrie. Un exemple clair : sur les blockchains comme Ethereum, des frais sont prélevés pour toutes les transactions, mais aucun créateur de contenu ne voudrait faire payer des frais aux utilisateurs pour commenter ou aimer ses articles. Si des SMT étaient basés sur Ethereum, ces frais seraient inévitables, ce qui disqualifie Ethereum en tant que plateforme de SMT.

Contrairement à Ethereum, certaines blockchains à programmabilité ouverte pourraient à l’avenir utiliser la limitation de bande passante comme frais de transaction, mais la limitation de la bande passante doit être ajustée précisément pour répondre aux exigences des applications spécifiques en termes d’UX. Par exemple, sur Steem, la limitation de la bande passante est spécialement conçue pour permettre le fonctionnement des applications de contenu et faciliter les interactions entre leurs utilisateurs en faisant varier les droits d’utilisation de la bande passante en fonction de deux éléments : la quantité de tokens détenus et la possession d’un compte. De plus, il a fallu plus d’un an de recherche au niveau de la production pour déterminer la bande passante optimale à attribuer à chacun. Sur les plateformes d’usage général à programmabilité ouverte, la nécessité d’établir un prix correct et la difficulté que cela représente peuvent diminuer la capacité des applications à attribuer un coût adéquat aux actions de leurs utilisateurs et le problème pourrait empirer au fur et à mesure de l’apparition de nouveaux prototypes d’applications, qui fragmenteraient et diviseraient les ressources de la blockchain. Dès lors, des blockchains qui prennent nativement en charge des applications spécifiques pourraient être plus aptes à déterminer les prix des transactions, comme ceux-ci influencent l’UX pour les tokens et les applications associées.

## Les SMT bénéficient d’une blockchain intégrant des processus d’extensibilité programmés pour une série d’applications spécialisées

Afin de rendre les blockchains extensibles, des concepts de pointe ont été inventés, tels que le "sharding" (apparu grâce à Vitalik Buterin et au projet Ethereum) et le "parallélisme multithread" (apparu grâce à Michael Vandenberg de Steem), qui désignent des façons d’étendre la blockchain en permettant à plusieurs opérations d’avoir lieu en même temps. Les plateformes d’usage général (comme Ethereum) sont un excellent moyen de tester ces façons d’approcher l’extensibilité, mais une plateforme comme Steem, qui tire parti des correspondances produit/marché découvertes par Ethereum et les applique à un modèle plus spécialisé caractérisé par des mises à jour progressives, peut adapter ses processus plus efficacement pour répondre à la demande révélée par cette correspondance produit/marché.

Si nous établissons une analogie avec les années 1990 et le début des années 2000, quand le monde de l’informatique a commencé à écrire du code optimisé spécialement pour les cartes graphiques, les limites des performances ont pu être repoussées grâce aux FPGA (*Field-Programmable Gate Array* ou circuits logiques programmables), des puces qui permettent de programmer les blocs logiques afin de former n’importe quel circuit, ce qui permet d’en faire, en substance, des prototypes d’ASIC (bien que leur consommation électrique soit supérieure). Elles n’ont pas la même performance par watt que les ASIC mais sont beaucoup plus rapides que les processeurs pour certaines tâches particulières. À mesure que les plateformes comme Ethereum procèdent de plus en plus à des généralisations, comme le fait qu’un contrat puisse faire appel à n’importe quel autre contrat, elles pourront de moins en moins être optimisées en vue d’une extension étant donné que les contrats qui font appel à d’autres contrats peuvent faire baisser la capacité de traitement multiparallèle jusqu’à ce que le traitement ne puisse plus s’effectuer que sur un seul coeur. Par analogie, tout comme les processeurs qui sont moins optimisés que les cartes graphiques, les plateformes telles que Tezos, GEOS et Ethereum sont moins optimisées que des blockchains "Turing-incomplètes" spécifiques à une application, telles que Steem. Ces blockchains analogues aux processeurs seront ralenties par des exigences de traitement imprévisibles, alors que les plateformes de blockchain optimales seront spécialisées, comme Steem, et seront extensibles grâce à des optimisations analogues aux optimisations des FPGA pour les algorithmes parallèles.

## Les SMT bénéficient d’une blockchain intégrant des primitives de système de gestion de contenu [(SGC/CMS)](https://en.wikipedia.org/wiki/Content_management_system)

Contrairement aux blockchains d’application générale comme Ethereum qui évitent par nature d’inclure des primitives spécifiques à une application au coeur de leur protocole, Steem offre une base de données de contenu public structurée servant à l’enregistrement de texte brut et de données structurées génériques ainsi que des primitives de contenu sur lesquelles les développeurs peuvent se baser : noms d’utilisateur, publications, commentaires, votes et solde du compte. Ces primitives sont utiles aux applications basées sur la blockchain, car elles aident à établir une interopérabilité entre les applications et permettent aux développeurs de se lancer rapidement. En l’absence de ces primitives, des bases de données additionnelles doivent être configurées spécialement pour chaque application basée sur la blockchain, ce qui peut entraîner une compétition entre une myriade de bases de données spécifiques aux applications. L’apparition de nombreuses bases de données de gestion de contenu diminue l’effet de réseau potentiel de la blockchain en tant que système de gestion de contenu (SGC) et réduit le potentiel d’interopérabilité des applications alors que celle-ci apporte des bénéfices en termes de sécurité du consommateur puisqu’elle permet aux utilisateurs finaux de passer facilement d’une application basée sur la blockchain à une autre.

# Augmentation de la demande du marché pour les STEEM grâce aux SMT et aux vecteurs de valeur implicite plutôt qu’aux frais 

Il y a plusieurs nouveaux vecteurs de valeur pour STEEM avec la création des SMT.

## Les STEEM dépensés pour la bande passante de transaction permettent une participation rentable au maximum parmi les SMT

Avec l’avènement des SMT, la demande de STEEM parmi les utilisateurs est croissante, parce que les utilisateurs doivent avoir de plus en plus de STEEM afin de pouvoir participer, consommer et utiliser les services Steem à un taux proportionnel au maximum à leur potentiel de croissance dans leurs écosystèmes SMT respectifs. En d’autres termes, à mesure que les utilisateurs expérimentés accroissent leur potentiel de gains dans les communautés SMT, ils doivent posséder plus de STEEM pour obtenir la quantité de bande passante leur permettant d’atteindre le plus haut taux de rendement possible dans les écosystèmes SMT. Au niveau applicatif, la demande de bande passante peut être satisfaite par les utilisateurs ou par les entreprises, qui peuvent déléguer de la bande passante excédentaire à leurs utilisateurs.

## Les STEEM sont bloqués dans des réserves de liquidité par les teneurs de marché automatisés

Chaque SMT qui exploite des teneurs de marché automatisés augmente la demande de STEEM par rapport aux quantités disponibles de STEEM. L’effet des teneurs de marché automatisés sur les STEEM est que chaque teneur de marché automatisé se constitue une réserve permanente de STEEM, ce qui entraîne une diminution des réserves disponibles. Si la demande reste inchangée, le prix du STEEM augmente à chaque fois qu’un nouveau teneur de marché automatisé apparaît.

## La demande de STEEM et de SMT augmente avec l’apparition de nouveaux pouvoirs d’influence

D’un point de vue potentiellement utilitaire, la demande de STEEM augmente à chaque création d’un SMT dans lequel le Steem Power a une influence partagée sur la réserve de récompenses du SMT. Si la réserve de récompenses d’un SMT subit une quelconque influence partagée basée sur le Steem Power, cela octroie de nouveaux droits et de nouvelles possibilités d’utilisation aux STEEM, ce qui provoque un accroissement la demande de STEEM. Ces droits peuvent également être accordés de SMT à SMT. Le flux de valeur suit un modèle identique.

## La demande de STEEM augmente avec la prolifération des ICO des SMT.

Au niveau de la plateforme, la demande peut aussi être causée par des opportunités de financement exclusives telles que les ICO. Ces dernières attirent de nouveaux capitaux dans les écosystèmes en passant d’abord par l’actif de base, le STEEM, puis par les SMT. L’augmentation du capital de l’écosystème grâce aux ICO offre toujours la possibilité qu’un capital positif net soit conservé en STEEM, et dans le pire des cas, on assiste à une remise à zéro de la valeur de l’actif de base, au cours de laquelle tous les STEEM sont vendus par l’organisation à l’origine de l’ICO. Exemple de scénario catastrophe : une ICO a lieu et 100 USD permettent d’acheter du STEEM pour acheter les SMT émis lors de l’ICO. 100 % des STEEM reçus par l’ICO sont ensuite vendus pour recevoir des USD. Il n’y a donc pas d’effet net explicite du point de vue de la valeur du STEEM. Toutefois, même si l’effet net de la contribution d’une ICO à la valeur du STEEM semble être nul, il y a un bénéfice net implicite en termes d’attention reçue par le STEEM et l’écosystème Steem, si nous considérons que toute attention à de la valeur. De plus, il est raisonnable de penser que, vu le comportement des ICO sur Ethereum, la majorité des STEEM reçus par les organisations qui ont fait des ICO continueront d’être détenus de manière spéculative ou à titre d’engagement, créant ainsi une valeur de quote-part.

## Steem : le réseau publicitaire mondial

En plus de ces nouveaux mécanismes créateurs de valeur, il est impératif de reconnaître la valeur originale créée pour le STEEM sous forme d’un réseau implicite d’attention et de publicité qui s’applique maintenant à tous les SMT qui utilisent les récompenses Proof-of-Brain. Les Smart Media Tokens, tout comme STEEM, ont des propriétés de curation inhérentes, les réserves de récompenses par exemple, qui leur offrent plus de fiabilité et de crédit en tant que réseau publicitaire implicite. La réserve de récompenses des SMT exige des interfaces auxquelles les SMT sont totalement intégrés, comme Steemit.com, qu’elles respectent les paiements en SMT en attente sur les publications, puis qu’elles classent ces publications selon les paiements en attente, des plus élevés aux plus bas, dans un onglet communément appelé « en vogue ». De cette manière, les publications peuvent être vérifiées par la communauté des personnes qui détiennent les SMT. Cela a pour résultat, et cela s’applique autant aux STEEM qu’aux futurs SMT, une page « en vogue » ordonnée que les utilisateurs (blogueurs, vlogueurs, publicitaires) peuvent utiliser de manière fiable pour évaluer les retours potentiels sur l’achat d’un emplacement en haut de la page pour mieux capter l’attention. Ensuite, les participants décident ***d’acheter ou de louer du STEEM et des SMT pour promouvoir du contenu***. À travers ce procédé, comme les publicitaires décident d’acheter et de louer du STEEM/SMT pour gagner en visibilité, la demande de STEEM/SMT augmente. Ces propriétés, qui sont vectrices de valeur, sont plus ou moins semblables à "Ethereum : l’ordinateur mondial". Mais dans ce cas-ci, il s’agirait plutôt de "Steem : le réseau publicitaire mondial".

# Assistance de l’écosystème Steem pour les SMT

## Intégration des SMT aux sites web et aux applications

### API et documentation

À mettre à jour continuellement pour les SMT. Les API actuelles de Steem existent ici :
[http://steem.readthedocs.io/en/latest/index.html](http://steem.readthedocs.io/en/latest/index.html)
et
[https://steemit.github.io/steemit-docs/](https://steemit.github.io/steemit-docs/)

### Outils partagés pour la création de comptes, la signature des clés et les fonctionnalités du portefeuille

Il existe plusieurs outils partagés pour prendre en charge les applications qui veulent externaliser l’inscription, la signature des transactions et les fonctionnalités du portefeuille, telles [SteemConnect](https://v2.steemconnect.com/). SteemConnect permet aux applications de prendre en charge les SMT tout en étant soutenues par des entrepreneurs qui ne sont pas forcément des experts en cryptomonnaie.

# Conclusion

Avec une combinaison de mesures spécifiques pour l’émission libre d’actifs, la limitation du taux de bande passante faisant office de coûts de transaction, la disponibilité permanente du contenu, la vitesse de transaction en temps réel, la distribution autonome de tokens, l’échange décentralisé, la tenue de marché automatisée et les contrats ICO, Steem présente le premier protocole de tokens pour les créateurs de contenu à travers l’Internet.

# Références bibliographiques

[1] Steemit, Inc., 2017. Steem Bluepaper. A protocol for bringing smart,
social currency to publishers and content businesses across the internet.
([https://www.steem.io/steem-bluepaper.pdf](https://www.steem.io/steem-bluepaper.pdf))

[2] Eyal Hertzog, Guy Benartzi & Galia Benartzi, 2017. Bancor Protocol.
Continuous Liquidity and Asynchronous Price Discovery for Tokens through
their Smart Contracts.
([https://about.bancor.network/static/bancor_protocol_whitepaper_en.pdf](https://about.bancor.network/static/bancor_protocol_whitepaper_en.pdf))

# Annexe

## Notes de mise en application

Voici une ligne du temps / diagramme états-transitions dans un lancement SMT :

![Timeline of implementation](img/timeline.png)
\begin{center}Figure 10: ligne du temps du lancement d’un SMT\end{center}

### Normes pour nommer les SMT

- Un nom de SMT doit être constitué de 3 à 10 lettres majuscules ASCII (A-Z).
- Le nom d’un SMT ne doit pas être `STEEM`, `SBD` ou `VESTS`.

### Normes des répertoires d’actifs

Un *répertoire* fait correspondre chaque IAN à un des états suivants : 

```
Listed
Deprecated
Unlisted
Blacklisted
```

Tous les noms d’actif possibles correspondent à l’un des états suivants: 

```
Free
Reserved
```

Un IAN `Listed` ou `Deprecated` a un nom qui lui est associé, qui doit être repris dans la liste en tant que `Reserved`.

Les interfaces utilisateur peuvent fournir une fonctionnalité *asset directory union* (rassemblement de répertoires d’actifs) pour élargir les répertoires en rassemblant plusieurs répertoires d’actifs en un seul répertoire d’actifs. Pour rassembler ces répertoires, il faut utiliser les algorithmes suivants pour résoudre des situations où un IAN est catégorisé différemment par des répertoires différents.

- (1) Si l’IAN est `Blacklisted` dans n’importe lequel des répertoires rassemblés, renvoyer `Blacklisted`.
- (2) Si l’IAN est `Listed` ou `Deprecated` dans plusieurs des répertoires rassemblés, et que tous ces registres ne sont pas d’accord sur le nom associé au SMT, renvoyer `Unlisted`.
- (3) Si l’IAN est `Listed` dans au moins un des répertoires rassemblés, renvoyer `Listed`.
- (4) Si l’IAN est `Deprecated` dans au moins un des répertoires rassemblés, renvoyer `Deprecated`.
- (5) Renvoyer `Unlisted`.

De même, voici les règles pour résoudre les noms catégorisés différemment dans différents répertoires :

- (1) Si le nom est `Reserved` dans n’importe lequel des répertoires rassemblés, renvoyer `Reserved`.
- (2) Renvoyer `Free`.

Un répertoire dynamique (basé sur une URL ou sur un compte de la blockchain) ne doit pas être mis en mémoire cache plus de 5 minutes.

### Directives des interfaces utilisateur pour les noms des SMT

- Une interface utilisateur peut, mais ce n’est pas obligatoire, avoir un répertoire d’actifs par défaut.
- Une interface utilisateur peut choisir de dissimuler les IAN non répertoriés.
- Une interface utilisateur doit permettre aux utilisateurs d’outrepasser ou de corriger les défauts des interfaces utilisateurs avec leurs propres répertoires d’actifs. 
- Une interface utilisateur doit reconsidérer le fait de masquer les IAN non répertoriés avec lesquels les utilisateurs ont fait beaucoup de transactions.

### Directives opérationnelles pour les répertoires d’actifs.

- Un répertoire d’actifs ne doit pas embrouiller les utilisateurs en utilisant un IAN bien connu pour qualifier un autre nom de SMT, ou en utilisant un nom de SMT bien connu pour qualifier un IAN différent.
- Un répertoire d’actifs doit rendre le répertoriage simple autant pour les créateurs de SMT qui cherchent à ajouter leur actif au répertoire que pour les développeurs des interfaces qui envisagent d’ajouter le répertoire à leur interface. 

### Formats des répertoires d’actifs

Les répertoires d’actifs URL ou fichier seront au format JSON. Les détails seront développés en même temps que la mise en œuvre. Les répertoires d’actifs basés sur la blockchain utiliseront une opération JSON spéciale. Encore une fois, les détails seront développés en même temps que la mise en œuvre.

## Tests unitaires

Les détails des test unitaires seront développés en même temps que la mise en oeuvre.
