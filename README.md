# Mecanismos de democracia directa en América Latina

Bienvenidos/as al repositorio GitHub de la base de datos "Mecanismos de democracia directa en América Latina" mantenida por integrantes del Observatorio de Reformas Políticas en América Latina.

## Contenidos

-   [Resumen](#resumen)
-   [Descripción](#descripción)
-   [Citado](#citado)
-   [Referencias](#referencias)

## Resumen

La base de datos contiene información obtenida mediante la consulta de la normativa que regula los mecanismos de democracia directa [iniciativa de ley ciudadana, revocación de mandato y consulta popular] de 17 países de América Latina entre 1979 y 2021.

La codificación de la información recolectada se realizó con base en las siguientes variables: país (nombre, cowcode y siglas), año en que se estableció la reforma, consecutivo de las reformas por país, norma que regula los mecanismos de democracia directa, existencia de la iniciativa de ley ciudadana, porcentaje de apoyo para promover la iniciativa ciudadana, exigencia de requisitos adicionales para promover la iniciativa ciudadana, existencia de la revocación de mandato presidencial, porcentaje de apoyo ciudadano para promover la revocación de mandato presidencial, exigencia de requisitos adicionales para promover la revocación de mandato presidencial, existencia de la revocación de mandato legislativa, porcentaje de apoyo ciudadano para promover la revocación de mandato legislativa, exigencia de requisitos adicionales para promover la revocación de mandato legislativa, promoción de consulta popular desde los poderes públicos, promoción de la consulta popular desde el ejecutivo, promoción de la consulta popular desde el legislativo, promoción de la consulta popular desde la ciudadanía y porcentaje de apoyo ciudadano para activar la consulta popular. 

Integrantes del Observatorio de Reformas Políticas en América Latina recopilaron y codificaron la información. Las personas responsables de la recopilación de los datos son Mariana Ramírez Bustamante (Universidad de Salamanca), Adrián Porras Flores (Universidad de Salamanca) y María de Guadalupe Salmorán Villar (Instituto de Investigaciones Jurídicas, UNAM); mientras que las personas responsables de la codificación de los datos son Carlos Guadarrama Cruz (Facultad de Estudios Superiores Acatlán, UNAM) y Elliot Román Almaraz (Facultad de Estudios Superiores Acatlán, UNAM).

## Descripción

El directorio `./Data/` contiene el archivo `./Data/DD_MecanismosDirecta` en el cual se encuentra toda la información relevante respecto a la base de datos de los mecanismos de democracia directa en América Latina. En específico, la base de datos se compone de las siguientes variables:

-   `país`: nombre del país en el cual se llevó a cabo la reforma al régimen electoral de la cámara baja en América Latina.

-   `cowcode`: código del país de acuerdo con la codificación de “Correlates of War”
https://correlatesofwar.org/data-sets/cow-country-codes.

-   `año_reforma`: año calendario al que corresponde la reforma a los mecanismos de democracia directa en cada país de América Latina entre 1979-2021.

-   `consec_reforma_pais`: registra el número consecutivo de las reformas a los mecanismos de democracia directa en cada país de América Latina. Ejemplo: Peru_1 Peru_2, Peru_3, Peru_4.

-   `norma`: indica el rango legal de la normatividad donde se establecen los mecanismos de democracia directa. Sus valores son Constitución [1]: los mecanismos de democracia directa están regulados en el marco constitucional; Ley [2]: los mecanismos de democracia directa están regulados en leyes electorales o en la materia.

-   `iniciativa_ley`: indica si la reforma establece el mecanismo de iniciativa ciudadana. Sus valores son No [0]: la reforma no menciona el mecanismo de iniciativa ciudadana; Sí [1]: la reforma regula el mecanismo de iniciativa ciudadana.

-   `porc_iniciativa`: indica el porcentaje de apoyos del padrón electoral (o censo electoral, según el país) que establece la norma para promover una iniciativa ciudadana.

-   `requi_adicion_iniciativa`: señala si la reforma establece requisitos adicionales al porcentaje de apoyo para promover una iniciativa de ley ciudadana. Sus valores son No [0]: la reforma no establece requisitos adicionales para promover este mecanismo de democracia directa y Sí [1]: la reforma establece requisitos adicionales para promover este mecanismo de democracia directa.

-   `revoca_presid`: indica si la reforma establece el mecanismo de revocación de mandato para la persona titular del poder ejecutivo. Sus valores son No [0]: la reforma no establece la revocación de mandato para la persona titular del poder ejecutivo y Sí [1]: la reforma establece la revocación de mandato para la persona titular del poder ejecutivo.

-   `porc_revoca_presid`: indica el porcentaje de apoyos del padrón electoral (o censo electoral, según el país) que establece la norma para promover la revocación de mandato de la persona titular del poder ejecutivo.

-   `requi_adicion_revoca_presid`: señala si la reforma establece requisitos adicionales al porcentaje de apoyo para promover la revocación de mandato de la persona titular del poder ejecutivo. Sus valores son No [0]: la reforma no establece requisitos adicionales para promover este mecanismo de democracia directa y Sí [1]: la reforma establece requisitos adicionales para promover este mecanismo de democracia directa.

-   `revoca_legis`: indica si la reforma establece el mecanismo de revocación de mandato para alguna persona perteneciente al poder legislativo. Sus valores son No [0]: la reforma no establece la revocación de mandato para alguna persona perteneciente al poder legislativo y Sí [1]: la reforma establece la revocación de mandato para alguna persona perteneciente al poder legislativo.

-   `porc_revoca_legis`: indica el porcentaje de apoyos del padrón electoral (o censo electoral, según el país) que establece la norma para promover la revocación de mandato de alguna persona perteneciente al poder legislativo.

-   `requi_adicion_revoca_legis`: señala si la reforma establece requisitos adicionales al porcentaje de apoyo para promover la revocación de mandato de alguna persona perteneciente al poder legislativo. Sus valores son No [0]: la reforma no establece requisitos adicionales para promover la revocación de alguna persona perteneciente al poder legislativo y Sí [1]: la reforma establece requisitos adicionales para promover la revocación de alguna persona perteneciente al poder legislativo.

-   `consult_poderes`: señala si la reforma establece la posibilidad de que los poderes públicos promuevan el mecanismo de consulta popular. Sus valores son No [0]: la reforma no establece la posibilidad de que los poderes públicos promuevan el mecanismo de consulta popular y Sí [1]: la reforma establece la posibilidad de que los poderes públicos promuevan el mecanismo de consulta popular.

-   `consult_ejecu`: señala si la reforma menciona que el poder ejecutivo podrá promover el mecanismo de consulta popular. Sus valores son No [0]: la reforma no menciona que el poder ejecutivo sea quien promueva el mecanismo de consulta popular y Sí [1]: la reforma menciona que el poder ejecutivo sea quien promueva el mecanismo de consulta popular.

-   `consult_legis`: señala si la reforma menciona que el poder legislativo podrá promover el mecanismo de consulta popular. Sus valores son No [0]: la reforma no menciona que el poder legislativo sea quien promueva el mecanismo de consulta popular y Sí [1]: la reforma menciona que el poder legislativo sea quien promueva el mecanismo de consulta popular.

-   `consult_ciudadania`: señala si la reforma menciona que la ciudadanía podrá promover el mecanismo de consulta popular. Sus valores son No [0]: la reforma no menciona que la ciudadanía sea quien promueva el mecanismo de consulta popular y Sí [1]: la reforma menciona que la ciudadanía sea quien promueva el mecanismo de consulta popular.

-   `porc_consult_ciudadania`: indica el porcentaje de apoyos del padrón electoral (o censo electoral, según el país) que establece la norma para promover la consulta popular.

## Citado

``` r
Freidenberg, Flavia. Dir., 2022, “Mecanismos de Democracia Directa en América Latina”, Observatorio de Reformas Políticas en América Latina (1978-2022). Ciudad de México: Instituto de Investigaciones Jurídicas (IIJ-UNAM) y Washington, D.C.: Secretaría para el Fortalecimiento de la Democracia de la Organización de los Estados Americanos (SFD/OEA), V2. DOI: https://doi.org/10.6084/m9.figshare.19078358.v2.
```