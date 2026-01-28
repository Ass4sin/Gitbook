# Roles d'hote

Tous les ordinateurs connectés à un reseau et qui participent directement au communications transmises sur le reseau sont des hotes. Les hotes sont aussi appeles des peripheriques finaux. Plus precisement une hote est une machine qui a une adresse ip attribué pour communiquer



## Peer-to-Peer

Quand un ordi fait office de serveur et de client sur le serveur on dit que le reseau est peer-to-peer

<figure><img src=".gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>



## Peripheriques intermediaires

Les peripheriques intermediaires connectent les peripheriques finaux sur le reseau



## Supports Reseau

Les reseaux modernes utilisent principalement 3 supports pour la connexion des peripheriques:

* Fils metalliques dans les cables: les donnes sont encodes en impulsions electriques
* Verre ou fibres plastiques (fibre optique): les donnes sont encodes en pulsations lumineuses
* Transmission sans fil : les donnes sont codes par modulations de frequence specifique d'ondes électromagnétiques

<figure><img src=".gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

## Representations du reseau

<figure><img src=".gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

En plus des icones il y a aussi des termes precis comme :

* NIC (Carte d'interface reseau) = Une NIC relie physiquement le dispositif terminal au reseau
* Port physique = Un port ou une prise sur un dispositif reseau qui ou le support se connecte a un autre dispositif terminal ou reseau
* Interface = Port specialise sur un dispositif reseau qui se connecte a des reseaux individuels. Exemple les ports sur le routeurs qui se connectent aux reseaux sont des interfaces de reseau

{% hint style="info" %}
Port et Interface sont souvent utilises l'un pour l'autre
{% endhint %}

## Diagramme de topologie

Diagramme de topologie physique: dans le schemas on voit l'emplacement des peripheriques

Diagramme de topologie logique: on voit a quoi les peripheriques sont connectes, quel interface, etc...

{% hint style="info" %}
fournisseur de service (PS) fournisseur de services Internet (ISP)
{% endhint %}

{% hint style="info" %}
L'Internet n'est la propriete de personne, pour cela plusieurs organisations se sont mis en place pour garder un ordre, comme Internet Engineering Task Force (IETF), Internet Corporation for Assigned Names and Numbers (ICANN), Internet Architecture Board (IAB) entre autres.
{% endhint %}

## Intranets et Extranets

Intranet est utilises pour parler d'une connexion prives de LAN et de WAN qui appartient a une organisation. Seuls les membres qui ont eu acces peuvent y aller

Une entreprise peut utiliser un extranet pour donnet acces sur et securise pour les personnes qui ont besoin des donnes et travaillent pour une autre organisation&#x20;

<figure><img src=".gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

## Internet

<mark style="color:$danger;">**C'est un reseau des reseaux, c'est l'ensemble de reseaux interconnectes**</mark>

{% hint style="info" %}
ADSL (Asymmetric Digital Subscriber Line)

DSL (Digital Subscriber Line)
{% endhint %}

## Connexions Internet des petits bureaux et des bureaux a domicile

<figure><img src=".gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

Un utilisateur a domicile va preferer le DSL et le cable, alors qu'un teletravailleur sera avec une connexion cellulaire. Pour finir les petits bureaux vont se connecter avec un satellite ou une ligne commutee

* **Câble** - Généralement proposé par les fournisseurs de services de télévision par câble, le signal de données Internet est transmis sur le même câble que celui qui achemine la télévision par câble. Il offre une large bande passante, une grande disponibilité et une connexion permanente à l'internet.
* **DSL** -Les lignes d'abonné numériques DSL offrent également une large bande passante, une grande disponibilité et une connexion permanente à l'internet. La technologie DSL utilise une ligne téléphonique. En général, un utilisateur de bureau à domicile ou de petit bureau se connecte à l'aide d'une ligne ADSL (Asymmetric Digital Subscriber Line), sur laquelle la vitesse descendante est supérieure à la vitesse ascendante.
* **Cellulaire** - L'accès à Internet par téléphone cellulaire utilise un réseau de téléphonie mobile pour se connecter. Partout où vous captez un signal cellulaire, vous pouvez accéder à Internet. Les performances sont limitées par les capacités du téléphone et de la tour de téléphonie cellulaire à laquelle il est connecté.
* **Satellite** - La disponibilité de l'accès à l'internet par satellite est un avantage dans les régions qui, autrement, n'auraient aucune connectivité internet. Les antennes paraboliques nécessitent une ligne de vue claire vers le satellite.
* **Ligne commutée** - Une option peu coûteuse qui utilise n'importe quelle ligne téléphonique et un modem. La faible bande passante des connexions par ligne commutée n'est généralement pas suffisante pour les transferts de données importants, mais cette solution reste utile pour accéder à Internet lors d'un déplacement.

## Connexion Internet d'entreprises

<figure><img src=".gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

* **Ligne louée dédiée** - Les lignes louées sont des circuits réservés au sein du réseau du fournisseur de services qui relient des bureaux géographiquement séparés pour un réseau privé de voix et/ou de données. Les circuits sont généralement loués sur une base mensuelle ou annuelle.
* **Metro Ethernet** - Ceci est parfois connu sous le nom Ethernet WAN. Dans ce module, nous l'appellerons Metro Ethernet. Les Metro ethernets étendent la technologie d'accès au LAN au WAN. Ethernet est une technologie LAN que vous découvrirez dans un autre module.
* **Business DSL** - Business DSL est disponible dans différents formats. Un choix populaire est la ligne d'abonné numérique symétrique (SDSL) qui est similaire à la version grand public de la DSL mais qui permet les téléchargements en amont et en aval aux mêmes vitesses élevées.
* **Satellite** - Le service par satellite peut fournir une connexion lorsqu'une solution câblée n'est pas disponible.

## Architecture du reseau

Pour garantir que un reseau fonctionne bien il y a 4 criteres:

* Tolerence aux pannes
* Evolutivite
* Quality of Service (QoS)
* Securite

## Tolerence aux pannes

Les reseaux tolerents aux pannes sont les reseaux qui limitent le nombre de dispositifs affectes lors d'une pane, et aussi a quelle vitesse on peut les remettre en place. Ces reseaux s'appuient sur le fait qu'il y'a pas qu'un seul peripherique reseau qui fait passer le message, si ce peripherique tombe un pane le message est envoye vers un autre lien. Le fait de disposer de plusieurs choix s'appelle la <mark style="color:$danger;">**redondance**</mark>

La mise en place d'un reseau a commutation de paquets est un des moyens avec lequel les reseaux fiables assurent la redondance. Un mail ou une video est coupe en plusieurs paquets que le reseau va commuter en fonction de l'etat du reseau. Les paquets peuvent prendre plusieurs chemins differents pour arriver a la meme destiantion.&#x20;

## Evolutivite

Un reseau evolutif se base sur le fait qu'on peut facilement ajouter un nouvel appareil au reseau sans **perturber** les anciens users. En outre, les reseaux sont evolutifs etant donne que les concepteurs font appel a des normes et a des protocoles reconnus.

## Quality of Service (QoS)

On peut parler de QoS quand on voit une video saccadee, les appels VOIP ont des problemes, etc... Les communications voix et video convergent sur le meme reseau, la QoS constitue consiste a faire en sorte que tout soit fluide pour l'user

Un encombrement survient lorsqu'une demande excessive de bande passante depasse les capacites disponibles. La bande passante reseau est mesure en fonction de nombre de bits passant par seconde (bit/s). Lorsque plusieurs communications sont initees en meme temps cela peut depasser la bande passante creant un encombrement du reseau.

Lorsque le volume du trafic est superieur a ce qui peut etre transmis les appareils gardent les paquets en memoire jusqu'a ce que des ressources soit disponibles pour les transmettre

<figure><img src=".gitbook/assets/QoS.png" alt=""><figcaption></figcaption></figure>

## Securite du reseau

L'infrastructure reseau, les services et les donnees stockees sur les peripheriques sont des actifs personnelles et professionnels essentiels. Les admin sys doivent s'ocuper de la securite du reseau et de la securite des informations

La securisation de l'infrastructure comprend la securisation physique des peripheriques et de la prevention de l'acces non autorise aux logiciels de gestion qui y resident

<figure><image src="./image.png"><figcaption></figcaption></figure>

Les admins sys doivent egalement proteger les informations dans les paquets transmis sur le reseau ainsi que les informations stockees sur les peripheriques connectes au reseau, pour cela on a 3 criteres:
    Confidentialite - seuls les destinataires prevus et autorises peuvent acceder aux donnes et les lire
    Integrite - les donnes n'ont pas ete modifie avant l'arrive
    Disponibilite - acces rapide et fluide aux services de donnees pour les users autorises