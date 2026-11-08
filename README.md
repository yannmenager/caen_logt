Méthodologie

Carte Carte_beta.html

L’objectif est d’estimer la densité de logements à l’échelle des îlots urbains de Caen, à partir de données ouvertes du cadastre, de la BD TOPO® de l’IGN et de la Base de données nationale des bâtiments (CSTB).

Les îlots sont délimités à l’aide du cadastre et de la BD TOPO®, en prenant notamment en compte les routes, les bâtiments et les zones d’activités. Des scripts SIG écrits avec Codex automatisent une partie de ces traitements.

Le nombre de logements recensés dans la BDNB est ensuite rattaché aux îlots. La BDNB s’appuie sur les fichiers fonciers du Cerema, eux-mêmes issus des bases MAJIC de la DGFiP : les logements comptabilisés sont donc des logements au sens fiscal.

Certains bâtiments de la BDNB sont représentés par plusieurs polygones, ce qui peut rendre leur attribution à un îlot incertaine. Ces situations sont repérées à l’aide de scripts, puis les contours des îlots sont retouchés pour réduire les incertitudes. Lorsqu’un bâtiment concerne plusieurs îlots et que son attribution ne peut pas être tranchée, la répartition est estimée au prorata de son emprise au sol. Les îlots concernés sont signalés afin d’indiquer les estimations les plus incertaines.

Cette méthode constitue un exercice exploratoire. Une utilisation opérationnelle nécessiterait notamment une expertise urbanistique pour valider les îlots, un contrôle exhaustif des résultats et une meilleure prise en compte de certains cas particuliers dans les données sources, comme les résidences étudiantes.

Sources des données : Base de données nationale des bâtiments (CSTB, version 2026-02-a, données des fichiers fonciers au 31-12-2025), BD TOPO® IGN (15-09-2026), Cadastre DGFiP par Etalab (01-09-2026)


Carte caen_dvf_beta.html

L’objectif était de qualifier un taux de mutation en calculant le nombre de maisons et d’appartements vendus par rapport au nombre total de logements sur chaque îlot, sur une période de 5 ans (du 01/01/2021 au 31/12/2025). Cette étude a été réalisée en utilisant exclusivement des données ouvertes, disponibles à l'échelle nationale. La méthode de création des îlots et de calcul du nombre de logements a été présentée ci-dessus.

La principale difficulté réside dans la nature des données utilisées : dans les bases DVF, les mutations immobilières sont affectées à une parcelle qui ne contient pas toujours les logements concernés. Ce ne sont pas des erreurs : la base originale répond à ses propres besoins, qui sont de nature fiscale. Par ailleurs, une transaction peut aussi concerner plusieurs parcelles éloignées, ce qui oblige à mener une analyse plus fine.
Des scripts ont donc été développés pour mesurer et réduire l’incertitude autant que possible, en étudiant la localisation des mutations par rapport aux îlots initiaux et en utilisant les contours des parcelles appartenant à des personnes morales, regroupées en unités foncières, car les mutations portant sur ces parcelles peuvent être sources d’erreurs.
Cela oblige à s’écarter d’une définition théorique stricte de l’îlot urbain et à modifier les îlots pour les adapter aux données.

La carte présente les résultats bruts des calculs automatiques, sans redressement. Comme pour la précédente publication, les chiffres doivent être pris avec du recul : ils devraient faire l’objet de contrôles plus nombreux, notamment pour corriger les biais liés aux données sources ou à la méthodologie et pour mieux qualifier les incertitudes.
