# Travailler avec un csv en SQL depuis dataCamp sans rien installer

Petite astuce pour travailler sans installer de serveur SQL, depuis datacamp en utilisant DataLab pour faire des requêtes SQL. 
Le plan gratuit permet d'avoir un petit DataLab

![datacamp01](./img/01.png)

## Transformer un csv en source SQL dans datacamp

Voici l'exemple avec le fichier csv des suicides en Inde que vous pouvez télécharger à [l'adresse officiel](https://www.kaggle.com/datasets/rajanand/suicides-in-india)

Télécharger le fichier csv sur votre machine (vous pourrez le supprimer ensuite)

Connecter vous à votre Datacamp:

![datacamp02](./img/02.png)

Allez dans DataLab, puis choissisez **Data Sources**

![datacamp03](./img/03.png)

Cliquez sur **New Data Source**

![datacamp04](./img/04.png)

Ici vous allez pouvoir faire un drag and drop du fichier csv que vous avez téléchargé précédemment

![datacamp05](./img/05.png)

La fenetre va s'agrandir d'un coup, déposer le fichier

![datacamp06](./img/06.png)

Le fichier va être importé sur le data source du dataLab

![datacamp07](./img/07.png)

Il sera ensuite analysé et un affichage des 100 premieres lignes sont proposées

![datacamp08](./img/08.png)

Cliquez ensuite sur le bouton **New Workbook**

![datacamp09](./img/09.png)

Vous avez ensuite un petit encard SQL qui vous permet de taper votre commande, en cliquant sur **Run** vous executez cette commande sur votre base de données fraichement montée.

![datacamp10](./img/10.png)

Ici je vérifie d'avoir le bon nombre d'enregistrement avec un *select count*

![datacamp11](./img/11.png)

le resultat de la commande est stocké dans un *dataframe* (ici df)

![datacamp12](./img/12.png)

comme vous pouvez le voir, avec un info sur le dataframe, on obtient les détails de celui-ci

![datacamp13](./img/13.png)

Ici je vais charger dans un data frame df1 la totalité de la table Suicide

![datacamp14](./img/14.png)

Je vérifie le contenu de mon dataframe

![datacamp15](./img/15.png)

Autre exemple de requete SQL

![datacamp16](./img/16.png)


## Transformer un csv depuis une base Mysql et s'y connecter depuis dataCamp

Il est possible d'avoir une base de données mysql gratuitement à l'adresse suivante: [Site officiel](https://freedb.tech/) 

![datacamp17](./img/17.png)

> Attention toutefois, on est limité à 100 connexions simultanément , il faut donc faire attention si vous importez le fichier suicide, depuis phpmyadmin, cela ne fonctionne pas.

> depuis dbeaver il faut décocher l'option "ouvrir connexion(s)" lors de l'import

Ensuite, dans votre *dataLab* rendez vous dans **data sources** comme précédemment et **New Data Source** puis choisissez **Mysql**

![datacamp18](./img/18.png)

Compléter les informations de connexion

![datacamp19](./img/19.png)

Vous aurez la validation de connexion, puis cliquez sur **continue**

![datacamp20](./img/20.png)

Et hop vous aurez cette fois-ci du pure SQL (par contre je ne sais pas le nombre de connexion qui sont ouvertes vers le serveur Mysql)

![datacamp21](./img/21.png)

Cliquez sur **New Workbook** et vous pouvez jouer avec du SQL

![datacamp22](./img/22.png)