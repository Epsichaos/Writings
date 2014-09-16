Développement sous Mac OS X
============================

De GNU/Linux à Mac OS X
------------------------

**Passer à Mac OS X après 5 ans de dual boot Windows - GNU/Linux**

Victime d'un BSOD fatal sous Windows XP, j'avais à l'époque décidé de passer à GNU/Linux, profitant de cette occasion pour découvrir et m'initier un peu à la programmation à l'aide de Ubuntu 9.04.

Aujourd'hui, après 5 ans de GNU/Linux, de dual boot, de multiples distributions (Backtrack, Fedora, Debian, Frugalware, Slackware, Slax, Arch Linux), je décide d'adopter un environnement de travail plus confortable, en passant sous Mac OS X.

Pourquoi un tel choix ? Lassé de nombreux problèmes rencontrés sous GNU/Linux (incompatibilité matérielle, configurations foireuses, problèmes réseau récurrents, ...) - et probablement causés par ma tendance à tout trifouiller - je décide donc de passer à Mac OS X, espérant que cette fois-ci, l'alliance matériel/OS soit "parfaite", et surtout, espérant avoir un linux, sans les heures de configuration qui vont avec.

Réinstaller un OS toutes les semaines, c'était amusant au début mais j'ai désormais besoin de qualité et de stabilité, sans avoir à configurer des heures, en naviguant de forum en forum pour trouver pourquoi la carte réseau déconne.

Passer à Mac OS X, c'était l'occasion de garder un environnement de travail agréable et similaire à GNU/Linux, avec un shell et des éditeurs de text convenable.

Logiciels indispensables
------------------------

**Se créér un environnement de développement agréable**

Lors de mon expérience linuxienne, j'avais pu profiter de très bon émulateurs de terminal, avec zsh et vim. Sous Mac OS X, il a fallu installer plusieurs logiciels et outils afin d'améliorer mon confort et de me rapprocher un peu de mon expérience passée.

Les logiciels et outils nécessaires au premier abord furent :

* iTerm2
* zsh
* brew
* git
* XCode
* Sublime Text 2 (ou 3)
* Google Chrome

1 - iTerm2
----------

iTerm2 est l'émulateur de terminal *ultime* pour Mac OS X. Si l'émulateur présent par défaut sur le système est d'une qualité plus que correcte, iTerm2 possède un grand nombre de fonctionalités supplémentaires très utiles : 

* Le mode plein écran, avec cmd + enter.
* L'Instant Replay, avec cmd + alt + B, on peut *voyager dans le temps* pour retrouver les anciennes commandes saisies précédemment.
* Un mode exposé pour les onglets (comme pour les fenêtres classiques).

Pour l'installer [iTerm2](http://iterm2.com/downloads.html)

Mettre iTerm en terminal par défaut : iTerm2 > Make iTerm2 default Shell.

2 - XCode
---------

XCode est l'IDE le plus connu de Mac OS X. Il permet notamment l'installation des outils de ligne de commande et de compilation - comme gcc - *non présents par défaut sous Mac OS X*. Plutôt peu pratique, je n'utilise d'IDE et il est assez lourd (presque 2Go X_x), plutôt pénible - mon Mac n'étant doté que d'un SSD à 256Go.

Il s'installe facilement et directement via l'AppStore.

3 - Git 
--------

L'installation de Git se fait en téléchargeant l'installateur sur le [Site officiel](https://mac.github.com/).

4 - Brew
---------

Homebrew est un gestionnaire de paquet pour Mac OS X, similaire au `apt-get` que l'on connaît bien chez Debian -  Ubuntu. Il est une alternative au très connu Macports.

Installation : Dans un terminal, saisir : 

	ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

Pour installer des paquets avec brew, rien de plus facile : 

	brew install nom_du_paquet

5 - Oh-my-zsh
--------------

Zsh est le shell par défaut dans Mac OS X. J'utilise le framework de configuration oh-my-zsh qui contient de merveilleux thèmes et plugins pour rendre iTerm2 encore plus convivial. Pour l'installer, taper dans un terminal :

	curl -L https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh | sh

J'utilise le thème Agnoster, avec les plugins osx, sublime (permet de lancer sublime text dans le terminal avec la commande *st*), git, github et brew (à modifier dans le ~/.zshrc). Pour le thème Agnoster, j'ai rencontré quelques problèmes qui ont nécessité l'installation de Powerline et des Powerline - Fonts.


6 - Powerline - Fonts
----------------------

[Powerline - Fonts](https://github.com/Lokaltog/powerline-fonts) permet d'utiliser Agnoster de manière convenable (contient des caractères non reconnus par les polices par défaut). J'utilise la police Sauce Code Powerline (anciennement Source Code Pro) dans iTerm2 et SublimeText 3.


7 - Outils et logiciels de développement
-----------------------------------------

* MAMP : Serveur apache pour Mac OS X.
* Python : Dernière version installée via brew.
* [Java](https://www.java.com/fr/) : Installation du dernier jre, sur le site officiel.

Sources
-------

Cet article se veut un condensé, une reformulation avec apport personnel, une adaptation de divers sites et articles trouvés lors de mon passage à OS X, dont voici les liens originaux :

* [Un environnement de développement Web sous Mac, de Ronan Guilloux](https://github.com/ronanguilloux/Writings/blob/master/draft/Un-environnement-de-developpement-web-sous-Mac.md)
