# Nom du projet
Nom du projet.

# Resume du projet.
Résumé du projet.

# montant_engage (variable cible)
Montant engagé par l'état pour financer le projet.

# Numero EJ
Numéro d'identification de l'établissement juridique (EJ) dans le répertoire Sirene.

# numero operateur
Numéro d'identification de l'opérateur économique dans le répertoire Sirene.

# Operateur
Nom de l'opérateur.

# Demarche
Identifiant de la démarche dans Démarches Simplifiées, la plateforme de dépôt des dossiers. Une démarche correspond à une thématique. Vous pouvez retrouver plus d'information sur ces démarches sur [le site de aides-territoires](https://aides-territoires.beta.gouv.fr/programmes/fonds-vert/).
Nom de la démarche dans Démarches Simplifiées.

# Nom Region
Nom de la région ayant engagé les crédits.

# Nom Departement
Nom du département ayant engagé les crédits.

# Code Departement
Code INSEE du département ayant engagé les crédits.

# Code Commune
Code INSEE de la commune du lieu d'implantation du projet si disponible, ou rattaché au porteur de projet. Cette colonne peut-être vide dans le cas de projets à échelle intercommunale, départementale ou régionale, même si certains RBOP ont choisi de noter le code commune du chef-lieu.

# Nom Commune
Nom de la commune associé au code_commune, selon le COG INSEE 2023.

# Axe
Identifiant de l'axe (ou action). Voir les différentes actions dans la description générale.

# Date Creation
Date de création de l'entreprise ou de l'établissement.

# Activite Principale
Activité principale de l'entreprise ou de l'établissement.

# NomenclatureActivitePrincipaleUniteLegale
Nomenclature d'activité de la variable activitePrincipaleUniteLegale.

Cette variable indique la nomenclature d'activité correspondant à la variable activitePrincipaleUniteLegale. Toutes les unités légales actives ont un code d'activité principale appartenant à la nomenclature la plus récente ; les unités légales cessées ont un code appartenant à la nomenclature en vigueur à la date de prise en compte de leur cessation. La variable nomenclatureActivitePrincipaleUniteLegale est à null si la variable activitePrincipaleUniteLegale est à null
Type
Historisé. Liste de codes, longueur 8, ou null.
NAFRev2
NAFRev1
NAF1993
NAP

https://www.sirene.fr/static-resources/documentation/v_sommaire_311.htm#2

# CategorieEntreprise

Catégorie d'entreprise de l'unité légale.

La catégorie d'entreprise est une variable statistique calculée par l'Insee. Ce n'est pas une variable du répertoire Sirene.

La variable categorieEntreprise est associée à une année de validité. Elle est mise à jour une fois par an (en juillet N+2 pour l’année N).
Type
Non-historisé. Liste de codes, de longueur 3.
Format :
PME : petite ou moyenne entreprise
ETI : entreprise de taille intermédiaire
GE : grande entreprise
null : donnée manquante ou "sans objet"

# CategorieJuridiqueUniteLegale
Catégorie juridique de l'unité légale.

La catégorie juridique est un attribut des unités légales. Pour une personne physique, elle vaut toujours 1000, que la personne soit artisan, commerçant, profession libérale, agriculteur ou autre, et ne peut changer ; pour les personnes morales, la catégorie juridique est susceptible d'évoluer au cours de la vie de l'entreprise.

Le code est attribué selon la nomenclature en vigueur, mais peut être à null (cas des unités purgées notamment). Le libellé associé aux codes des catégories juridiques n'est pas historisé : pour les unités cessées à une date antérieure à l'entrée en vigueur de la derniere nomenclature, le libellé « Hors nomenclature » est affiché.
Type
Historisé. Liste de codes, de longueur 4.

# trancheEffectifsUniteLegale
Tranche d'effectif salarié de l'unité légale.

Il s'agit d'une variable statistique mise à jour une fois par an. Sa valeur est calculée à partir des données connues au 31 décembre de l’année millésime N (anneeEffectifsUniteLegale) et diffusée l’année N+2, généralement à l’automne.
Type
Non-historisé. Liste de codes, de longueur 2.

Modalités :
NN : Unité non-employeuse ou présumée non-employeuse (faute de déclaration reçue)
00 : 0 salarié (n'ayant pas d'effectif au 31/12 mais ayant employé des salariés au cours de l'année N)
01 : 1 ou 2 salariés
02 : 3 à 5 salariés
03 : 6 à 9 salariés
11 : 10 à 19 salariés
12 : 20 à 49 salariés
21 : 50 à 99 salariés
22 : 100 à 199 salariés
31 : 200 à 249 salariés
32 : 250 à 499 salariés
41 : 500 à 999 salariés
42 : 1 000 à 1 999 salariés
51 : 2 000 à 4 999 salariés
52 : 5 000 à 9 999 salariés
53 : 10 000 salariés et plus

# SocieteMissionUniteLegale
Appartenance au champ des sociétés à mission.

Cette variable indique si l'entreprise appartient au champ des sociétés à mission. L'article 176 de la loi du 22 mai 2019 relative à la croissance et la transformation des entreprises, dite loi Pacte, introduit la qualité de société à mission. Il permet à une société de faire publiquement état de la qualité de société à mission en précisant sa raison d'être ainsi qu’un ou plusieurs objectifs sociaux et environnementaux que la société se donne pour mission de poursuivre dans le cadre de son activité.
Type
Historisé. Liste de codes, de longueur 1, ou null.

Modalités :
O : l'entreprise appartient au champ des sociétés à mission ;
N : l'entreprise n'appartient pas au champ des sociétés à mission


# EtatAdministratifEtablissement
Etat administratif de l'établissement.

Lors de son inscription au répertoire, un établissement est, sauf exception, à l'état Actif. Le passage à l'état Fermé découle de la prise en compte d'une déclaration de fermeture. Un établissement fermé peut être rouvert. En règle générale, la première période d'historique d'un établissement correspond à un etatAdministratifUniteLegale égal à Actif. Toutefois, l'état administratif peut être à null (première date de début de l'état postérieure à la première date de début d'une autre variable historisée).
Type
Historisé. Liste de codes, de longueur 1, format :
A : Actif
F : Fermé

# AnneeEffectifsEtablissement
Année de validité de la tranche d'effectif salarié de l'établissement.

La mise à jour des tranches d'effectifs est annuelle (automne). Pour les établissements dont la tranche d’effectifs est renseignée, l’année de validité correspondante est l’année millésime N (voir trancheEffectifsEtablissement). Il n'y a jamais plus d’un seul millésime présent dans la base Sirene.
Type
Non-historisé. Date, de longueur 4, format AAAA, ou null.

# EconomieSocialeSolidaireUniteLegale
Appartenance au champ de l'économie sociale et solidaire.

Cette variable indique si l'entreprise appartient au champ de l'économie sociale et solidaire. La loi n° 2014-856 du 31 juillet 2014 définit officiellement le périmètre de l'économie sociale et solidaire (ESS). Celle-ci comprend les quatre familles traditionnelles en raison de leur régime juridique (associations, fondations, coopératives et mutuelles) et inclut une nouvelle catégorie, les entreprises de l'ESS, adhérant aux mêmes principes :
poursuivre un but social autre que le seul partage des bénéfices ;
un caractère lucratif encadré (notamment des bénéfices majoritairement consacrés au maintien et au développement de l'activité) ;
une gouvernance démocratique et participative.
Cette variable est renseignée pour environ 1 million d'entreprises, sinon null.
Type
Historisé. Liste de codes, de longueur 1, ou null.

Modalités :
O : l'entreprise appartient au champ de l'économie sociale et solidaire ;
N : l'entreprise n'appartient pas au champ de l'économie sociale et solidaire.

