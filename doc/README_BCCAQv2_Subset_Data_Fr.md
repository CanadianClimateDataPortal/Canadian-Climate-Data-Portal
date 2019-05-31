# BCCAQv2
## Annuel

Ces fichiers contiennent les valeurs annuelles pour les années 1950 à 2100 de la variable et de le point de grille que vous avez sélectionnés.  Les valeurs des données dans ces fichiers sont les mêmes que celles utilisées pour tracer les cartes affichées dans la section géoréférencée du site DonneesClimatiques.ca et en effectuant un zoom sur un seul point de grille à partir des cartes affichées dans la section à base de variables. Ces valeurs de données résument les climats simulés d'un ensemble de 24 modèles climatiques qui constituent l'ensemble de données BCCAQv2. La composante historique du climat simulé couvre la période 1950-2005, tandis que les projections futures pour les RCP 2.6, 4.5 et 8.5 sont de 2006 à 2100. Pour la composante historique et les projections futures, il y a trois colonnes : Médiane (50e percentile), intervalle (faible) - 10e percentile et intervalle (élevé) - 90e percentile.

Les fichiers csv contiennent 13 colonnes de données, la colonne 1 indiquant la date (p. ex. 1950-01-01-01 ; chaque ligne représente une seule année) et les colonnes suivantes fournissant les résultats de la simulation historique (colonnes 2-4), RCP 2.6 (colonnes 5-7), RCP 4.5 (colonnes 8-10) et RCP 8.5 (colonnes 11-13). La ligne d'en-tête identifie les valeurs de simulation et de percentile.
 
 
## Quotidien

Les données quotidiennes de l'ensemble de données BCCAQv2 peuvent être téléchargées en format csv ou NetCDF pour la période 1950-2100. Les fichiers au format NetCDF exigent que l'utilisateur soit familier avec des applications telles que R ou Python pour pouvoir lire et manipuler les données contenues dans ces fichiers.

Quel que soit le format de fichier, ces fichiers de données contiennent les résultats quotidiens des 24 modèles climatiques individuels qui composent l'ensemble de données BCCAQv2. Celles-ci sont énumérées dans le tableau 1.

Les trois premières colonnes des fichiers au format csv indiquent la date (année-mois-jour), la latitude et la longitude, et ce respectivement. Chacune des colonnes suivantes représente un seul modèle climatique et un seul RCP, la ligne d'en-tête de chaque colonne identifiant le nom de la variable, le modèle climatique et le RCP. Chaque ligne du fichier csv après cette ligne d'en-tête représente un seul jour.

Tous les modèles climatiques n'ont pas le même nombre de jours dans leur année modèle. Par exemple, les modèles du Royaume-Uni Met. Office Hadley Centre (HadGEM2) ont une année de 360 jours se composant de 12 mois chacun avec 30 jours. Certains modèles ont une année de 365 jours, mais n'incluent pas les années bissextiles. Alors que d'autres utilisent le calendrier standard de 365 jours pour les années non bissextiles et tous les quatre ans avec une année de 366 jours. 

Lors du téléchargement des données quotidiennes au format csv, vous recevrez un fichier zip qui contient quatre fichiers csv, comme suit :

1.	*_360_day.csv - ce fichier contient les modèles ayant une année de 360 jours, avec 12 mois contenant chacun 30 jours.
2.	*_365_day.csv - ce fichier contient les modèles ayant une année de 365 jours, et aucune année bissextile.
3.	*_standard.csv - ce fichier contient les modèles qui ont 365 jours par an et chaque quatrième année est une année bissextile contenant 366 jours.
4.	*_propleptic_gregorian.csv - ce fichier contient les modèles qui ont 365 jours par an et chaque quatrième année est une année bissextile contenant 366 jours.

Voici la liste des modèles climatiques et des centres de modélisation: **BNU-ESM** par Beijing Normal University, **CCSM4** par US National Center for Atmospheric Research, **CESM1-CAM5** par NSF-DOE-NCAR, **CNRM-CM5** par Centre National de Recherches Météorologiques et Centre Européen de Recherche et Formation Avancées en Calcul Scientifique, **CSIRO-Mk3-6-0** par Queensland Climate Change Centre of Excellence and Commonwealth Scientific and Industrial Research Organisation, **CanESM2** par Canadian Centre for Climate Modelling and Analysis, **FGOALS-g2** par LASG (Institute of Atmospheric Physics) – CESS (Tsinghua University), **GFDL-CM3**, **GFDL-ESM2G** et **GFDL-ESM2M** par NOAA Geophysical Fluid Dynamics Laboratory, **HadGEM2-AO** et **HadGEM2-ES** par UK Met Office Hadley Centre, **IPSL-CM5A-LR** et **IPSL-CM5A-MR** par Institut Pierre Simon Laplace, **MIROC-ESM**, **MIROC-ESM-CHEM** et **MIROC5** par University of Tokyo, National Institute for Environmental Studies and Japan Agency for Marine-Earth Science and Technology, **MPI-ESM-LR** et **MPI-ESM-MR** par Max Planck Institute for Meteorology, **MRI-CGCM3** par Meteorological Research Institute, **NorESM1-M** et **NorESM1-ME** par Norwegian Climate Centre et **bcc-csm1-1** et **bcc-csm1-1-m** par Beijing Climate Centre, China Meteorological Administration.
 
Le tableau 9.A.1 du chapitre 9 du cinquième rapport d'évaluation du GIEC fournit de plus amples détails et des références pour chacun des modèles climatiques : [Climate Change 2013: The Physical Science Basis](https://www.ipcc.ch/report/ar5/wg1). (Lien en anglais)
