Méthodologie

L’objectif est d’estimer la densité de logements à l’échelle des îlots urbains de Caen, à partir de données ouvertes du cadastre, de la BD TOPO® de l’IGN et de la Base de données nationale des bâtiments (BDNB).

Les îlots sont délimités à l’aide du cadastre et de la BD TOPO®, en prenant notamment en compte les routes, les bâtiments et les zones d’activité. Des scripts SIG écrits avec Codex automatisent une partie de ces traitements.

Le nombre de logements recensés dans la BDNB est ensuite rattaché aux îlots. La BDNB s’appuie sur les fichiers fonciers du Cerema, eux-mêmes issus des bases MAJIC de la DGFiP : les logements comptabilisés sont donc des logements au sens fiscal.

Certains bâtiments de la BDNB sont représentés par plusieurs polygones, ce qui peut rendre leur attribution à un îlot incertaine. Ces situations sont repérées à l’aide de scripts, puis les contours des îlots sont retouchés pour réduire les incertitudes. Lorsqu’un bâtiment concerne plusieurs îlots et que son attribution ne peut pas être tranchée, la répartition est estimée au prorata de son emprise au sol. Les îlots concernés sont signalés afin d’indiquer les estimations les plus incertaines.

Cette méthode constitue un exercice exploratoire. Une utilisation opérationnelle nécessiterait notamment une expertise urbanistique pour valider les îlots, un contrôle exhaustif des résultats et une meilleure prise en compte de certains cas particuliers dans les données sources, comme les résidences étudiantes.

Sources des données : Base de données nationale des bâtiments (version 2026-02-a, données des fichiers fonciers au 31-12-2025), BD TOPO® IGN (15-09-2026), Cadastre DGFiP par Etalab (01-09-2026)
