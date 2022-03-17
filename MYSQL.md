**CFGS Administració de Sistemes Informàtics a la Xarxa**

**Mòdul 10:** Administració de sistemes gestors de base de dades (ASIX)

**UF 1:** Llenguatges SQL: DCL i extensió procedimental

SGBD corporatiu

**Activitat 1: Instal·lació SGBD**

**Gaurav Pal**

**Ahmed Belhadi**

**ASIX**

**16/03/2022**


# **[ABANS DE LA INSTAL·LACIÓ]{.underline}** 

1.  Primer abans de res, ens creem una copte d'usuari en la web de
    RedHat: <https://access.redhat.com/tags/login>

2.  Ara, iniciem la subscripció i activem la llicencia de 60 dies

![Interfaz de usuario gráfica, Texto, Aplicación Descripción generada
automáticamente](./images//media/image1.png){width="6.686805555555556in"
height="1.2569444444444444in"}

![Interfaz de usuario gráfica, Texto, Aplicación Descripción generada
automáticamente](./images//media/image2.png){width="6.686805555555556in"
height="1.8652777777777778in"}

3.  Esborrem la subscripció que havia tingut prèviament ![Texto
    Descripción generada
    automáticamente](./images//media/image3.png){width="6.267442038495188in"
    height="0.6624311023622047in"}

4.  Deixem de registrar-nos a l'antic compte

![Texto Descripción generada
automáticamente](./images//media/image4.png){width="6.220833333333333in"
height="0.5229166666666667in"}

5.  Eliminem la suscrpció

![](./images//media/image5.png){width="6.220833333333333in"
height="0.3951388888888889in"}

6.  Ara fiquem el codi següent, per tal de connectar-se via consola:

![Texto Descripción generada
automáticamente](./images//media/image6.png){width="6.325694444444444in"
height="1.1395833333333334in"}

> ![Texto Descripción generada
> automáticamente](./images//media/image7.png){width="6.325694444444444in"
> height="0.5347222222222222in"}

# **[PART II -- INSTAL·LACIÓ SGBD MySQL 8.0]{.underline}** 

Per fer la instal·lació primer descarreguem el rpm del MYSQL

![Texto Descripción generada
automáticamente](./images//media/image47.png){width="5.90625in"
height="2.09375in"}

Després instal·lem el rpm en dirà si volem acceptar i li donem que si

![Texto Descripción generada
automáticamente](./images//media/image48.png){width="5.90625in"
height="2.3125in"}

Comprovem amb aquesta comanda si estan els repositoris

![Texto Descripción generada
automáticamente](./images//media/image49.png){width="5.90625in"
height="0.875in"}

Activem els repositoris y per això tindrem que desactivar els mòduls es
dirà si volem desactivar-lo i li diem que si![Texto Descripción generada
automáticamente](./images//media/image50.png){width="5.90625in"
height="2.0833333333333335in"}

Una vegada desactivat el mòdul ja podem instal·lar el MYSQL

![](./images//media/image51.png){width="5.90625in" height="0.71875in"}

Ens dirà si volem instal·lar-lo i li donem que si

![Forma, Rectángulo Descripción generada
automáticamente](./images//media/image52.png){width="5.90625in"
height="0.8645833333333334in"}

Ens dirà si volem instal·lar les claus importades i li donem que si a
tot i amb això ja tindrem instal·lat el MYSQL

![Texto Descripción generada
automáticamente](./images//media/image53.png){width="5.90625in"
height="2.0520833333333335in"}

**A on es troben físicament els fitxers de dades?** Els fitxers de dades
del MYSQL es troben a /var/lib/mysql/

**A on es troba el fitxer de configuració? Quin és el seu contingut?**

El fitxer de configuració del MySQL és troba en /etc/my.cnf. Per sabé el
que conte el fitxer de configuració anem a aquesta ruta i modifiquem el
arxiu

![](./images//media/image54.png){width="3.1770833333333335in"
height="0.3333333333333333in"}

El que conté el fitxer de configuració són buffers i diverses rutes del
mysql.![Texto Descripción generada
automáticamente](./images//media/image55.png){width="5.90625in"
height="4.625in"}

El procés de mysqld escolta al port 3306.

Els passos que faríem per canviar el port per defecte de MYSQL 3306 a
33306 son les següents:

Primer parem el servei de MYSQL

![](./images//media/image41.png){width="3.5208333333333335in"
height="0.15625in"}

I després anem a la ruta de configuració del percona.

![](./images//media/image42.png){width="3.6354166666666665in"
height="0.2916666666666667in"}

I si no hi ha port posem el port 33306 i ho guardem.

![Texto Descripción generada
automáticamente](./images//media/image43.png){width="4.53125in"
height="1.5625in"}

Engeguem el servei del mysql

![](./images//media/image44.png){width="3.5104166666666665in"
height="0.2604166666666667in"}

Fem una securització

![Interfaz de usuario gráfica, Texto Descripción generada
automáticamente](./images//media/image45.png){width="4.270833333333333in"
height="0.8541666666666666in"}

Entrem al mysql y posem la comanada per veure si ha canviat el port on
esta marcat que tindria que ser el 33306 i així es canviaria el port.

![Texto Descripción generada
automáticamente](./images//media/image46.png){width="5.572916666666667in"
height="3.0729166666666665in"}

Un cop finalitzada la instal·lació i veure que funciona, mostra el
resultat de la comanda:

![Texto Descripción generada automáticamente con confianza
media](./images//media/image56.png){width="5.90625in"
height="0.71875in"}

Webgrafia:

-   <https://computingforgeeks.com/how-to-install-percona-mysql-server-on-centos-rhel/#:~:text=%20Install%20Percona%20MySQL%20Server%208%20on%20CentOS,installation%20created%20a%20new%20repository%20file...%20More%20>

-   <https://www.linkedin.com/pulse/how-change-mysql-default-port-3306-secure-piyush-diwakar?msclkid=051592a2a53f11ecb903621e37f5ee4f>

-   <https://dev.mysql.com/doc/refman/8.0/en/installing.html>

