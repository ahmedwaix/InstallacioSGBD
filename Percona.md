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
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image1.png)
(https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image2.png){width="6.686805555555556in"
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

# **[PART I -- INSTAL·LACIÓ SGBD MySQL Percona Server]{.underline}** 

Primer de tot tindrem que instal·lar el repositori de Percona

![](./images//media/image8.png){width="5.90625in" height="0.25in"}

![Texto Descripción generada
automáticamente](./images//media/image9.png){width="5.90625in"
height="1.3229166666666667in"}

Ens demanarà si estem d'accords amb l'instal·lació, li diem que si

![Texto Descripción generada
automáticamente](./images//media/image10.png){width="5.90625in"
height="1.9791666666666667in"}

Activem els repositori, per fer-ho utilitzem la següent comanda:

![](./images//media/image11.png){width="2.6875in" height="0.28125in"}

![](./images//media/image12.png){width="5.90625in"
height="0.2708333333333333in"}

Seguidament ens preguntarà si volem desactivar els mòdul dfn, li donem
que si

![](./images//media/image13.png){width="5.90625in"
height="0.4270833333333333in"}

Instal·lem els paquets de Percona

![](./images//media/image14.png){width="3.1666666666666665in"
height="0.3854166666666667in"}

![Texto Descripción generada
automáticamente](./images//media/image15.png){width="5.90625in"
height="1.0104166666666667in"}

![Texto Descripción generada
automáticamente](./images//media/image16.png){width="5.90625in"
height="6.177083333333333in"}

Ens mostrarà el tamany de la descàrrega i si estem d'acords amb la
instal·lació, li donarem a si.

![Interfaz de usuario gráfica, Texto, Aplicación Descripción generada
automáticamente](./images//media/image17.png){width="3.0208333333333335in"
height="0.6458333333333334in"}

Ens demanarà si estem d' acord en importar claus li donarem tot que si i
ja tindrem el Percona server instal·lat

![Texto Descripción generada
automáticamente](./images//media/image18.png){width="5.90625in"
height="2.8541666666666665in"}

Un cop realitzada la instal·lació realitza una securització de la
mateixa. Per fer la tasca s'ha utilitzat el mysql_secure_installation

Per fer la securització primer tenim que utilitzar la següent comanda:

![](./images//media/image19.png){width="5.90625in"
height="0.19791666666666666in"}

I ens crearà una contrasenya provisional

![](./images//media/image20.png){width="5.90625in"
height="0.6354166666666666in"}

Ara que ja tenim la contrasenya provisional ja podem utilitzar la
comanda i ens demanarà el password provisional:

![Texto Descripción generada
automáticamente](./images//media/image21.png){width="4.385416666666667in"
height="1.2395833333333333in"}

Ens demanarà una nova contrasenya i posem una contrasenya provisional ja
que no deixarà posar la contrasenya patata per la política de
contrasenyes del mysql

![Texto Descripción generada
automáticamente](./images//media/image22.png){width="5.90625in"
height="0.78125in"}

Posarem la comanda per veure les dues política de contrasenya que tenim
que canviar

![Escala de tiempo Descripción generada automáticamente con confianza
media](./images//media/image23.png){width="4.375in" height="2.21875in"}

Canviem la política de contrasenyes a low i li posem un length de 6 amb
això podrem posar la contrasenya 'patata'

![](./images//media/image24.png){width="5.260416666666667in"
height="0.46875in"}

![](./images//media/image25.png){width="5.208333333333333in"
height="0.4583333333333333in"}

I ara si podrem cambiar el password a "patata" amb aquesta comanda

![Texto Descripción generada
automáticamente](./images//media/image26.png){width="4.177083333333333in"
height="0.8229166666666666in"}

Ara farem les les instruccions per arrancar / verificar status / apagar
servei de la base de dades de Percona Server del sistema operatiu:

Per arrancar el mysql utilitzarem aquesta comanda

![Texto Descripción generada
automáticamente](./images//media/image27.png){width="4.6875in"
height="0.5625in"}

I per apagar el mysql utilitzarem aquesta comanda

![Texto Descripción generada
automáticamente](./images//media/image28.png){width="4.041666666666667in"
height="0.5416666666666666in"}

Per verificar el estatus utilitzarem aquesta comanda

![Texto Descripción generada
automáticamente](./images//media/image29.png){width="5.90625in"
height="2.6041666666666665in"}

**On es troba i quin nom rep el fitxer de configuració del SGBD Percona
Server?**

El fitxer de configuració utilitzat per gestionar Percona Server per a
MySQL és troba en /etc/my.cnf. i rep el nom de my.cnf.

**A on es troben físicament els fitxers de dades (per defecte). Com ho
has sabut?**

Percona Server per MySQL emmagatzema els fitxers de dades a
/var/lib/mysql/ per defecte, això ho hem sabut gràcies a la documentacio
oficial de percona.

![Interfaz de usuario gráfica, Aplicación Descripción generada
automáticamente](./images//media/image30.png){width="5.90625in"
height="1.1979166666666667in"}

Crea un usuari anomenat asix en el sistema operatiu i en SGBD de tal
manera que aquest usuari del sistema operatiu no hagi d\'introduir
l\'usuari i password cada vegada que cridem al client mysql

Creem el usuari asix

![](./images//media/image31.png){width="3.1041666666666665in"
height="0.4895833333333333in"}

Quan intentem canviar la contrasenya ens diu que no podem, tenim que
tenir mínim 8 caràcters així que tindrem que canviar la política de
contrasenyes en el sistema operatiu.

![Interfaz de usuario gráfica, Texto, Sitio web Descripción generada
automáticamente](./images//media/image32.png){width="5.791666666666667in"
height="0.90625in"}

Per canviar la política tenim que anar a la següent ruta

![](./images//media/image33.png){width="4.208333333333333in"
height="0.40625in"}

I obrim el arxiu de configuració de la política de contrasenyes

![Texto Descripción generada
automáticamente](./images//media/image34.png){width="5.90625in"
height="1.0833333333333333in"}

Busquem el apartat de la longitud de la contrasenya y ho canviem a 6 y
ho guardem

![Texto Descripción generada
automáticamente](./images//media/image35.png){width="5.90625in"
height="2.0625in"}

I ara ja podem canviar la contrasenya a "patata"

![Texto Descripción generada
automáticamente](./images//media/image36.png){width="5.90625in"
height="0.9791666666666666in"}

Creem el usuari asix amb la contrasenya patata dins del mySQL del root

![Texto Descripción generada
automáticamente](./images//media/image37.png){width="5.552083333333333in"
height="3.2916666666666665in"}

Per poder accedir al Mysql sense password del usuari Asix primer tindrem
que crear un arxiu de configuració en la ruta següent

![](./images//media/image38.png){width="5.458333333333333in"
height="0.28125in"}

Y dins del fitxer de configuració posem el script de la contrasenya i ho
guardem

![Texto Descripción generada
automáticamente](./images//media/image39.png){width="5.90625in"
height="3.4583333333333335in"}

Ja podem accedir al mysql del asix sense contrasenya:

![Texto Descripción generada
automáticamente](./images//media/image40.png){width="6.395833333333333in"
height="2.3854166666666665in"}

El servei de MySQL (mysqld) escolta al port 3306.

Els passos que faríem per canviar el port per defecte de mysql 3306 a
33306 son les següents:

Primer parem el servei de mysql

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

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image44.png)

Fem una securització

![Interfaz de usuario gráfica, Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image45.png)

Entrem al mysql y posem la comanada per veure si ha canviat el port on
esta marcat que tindria que ser el 33306 i així es canviaria el port.

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image46.png)

Webgrafia:

-   <https://computingforgeeks.com/how-to-install-percona-mysql-server-on-centos-rhel/#:~:text=%20Install%20Percona%20MySQL%20Server%208%20on%20CentOS,installation%20created%20a%20new%20repository%20file...%20More%20>

-   <https://www.linkedin.com/pulse/how-change-mysql-default-port-3306-secure-piyush-diwakar?msclkid=051592a2a53f11ecb903621e37f5ee4f>

-   <https://www.percona.com/doc/percona-server/8.0/index.html>

