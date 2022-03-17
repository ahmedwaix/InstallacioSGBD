**CFGS Administració de Sistemes Informàtics a la Xarxa**

**Mòdul 10:** Administració de sistemes gestors de base de dades (ASIX)

**UF 1:** Llenguatges SQL: DCL i extensió procedimental

SGBD corporatiu

**Activitat 1: Instal·lació SGBD**

**Gaurav Pal**

**Ahmed Belhadi**

**ASIX**

**16/03/2022**

# **[ABANS DE LA INSTAL·LACIÓ]** 

1.  Primer abans de res, ens creem una copte d'usuari en la web de
    RedHat: <https://access.redhat.com/tags/login>

2.  Ara, iniciem la subscripció i activem la llicencia de 60 dies

![Interfaz de usuario gráfica, Texto, Aplicación Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image1.png)
![Interfaz de usuario gráfica, Texto, Aplicación Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image2.png)

3.  Esborrem la subscripció que havia tingut prèviament ![Texto
    Descripción generada
    automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image3.png)

4.  Deixem de registrar-nos a l'antic compte

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image4.png)

5.  Eliminem la suscrpció

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image5.png)

6.  Ara fiquem el codi següent, per tal de connectar-se via consola:

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image6.png)

> ![Texto Descripción generada
> automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image7.png)

# **[PART I -- INSTAL·LACIÓ SGBD MySQL Percona Server]** 

Primer de tot tindrem que instal·lar el repositori de Percona

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image8.png)

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image9.png)

Ens demanarà si estem d'accords amb l'instal·lació, li diem que si

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image10.png)

Activem els repositori, per fer-ho utilitzem la següent comanda:

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image11.png)

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image12.png)

Seguidament ens preguntarà si volem desactivar els mòdul dfn, li donem
que si

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image13.png)

Instal·lem els paquets de Percona

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image14.png)

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image15.png)

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image16.png)

Ens mostrarà el tamany de la descàrrega i si estem d'acords amb la
instal·lació, li donarem a si.

![Interfaz de usuario gráfica, Texto, Aplicación Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image17.png)

Ens demanarà si estem d' acord en importar claus li donarem tot que si i
ja tindrem el Percona server instal·lat

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image18.png)

Un cop realitzada la instal·lació realitza una securització de la
mateixa. Per fer la tasca s'ha utilitzat el mysql_secure_installation

Per fer la securització primer tenim que utilitzar la següent comanda:

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image19.png)

I ens crearà una contrasenya provisional

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image20.png)

Ara que ja tenim la contrasenya provisional ja podem utilitzar la
comanda i ens demanarà el password provisional:

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image21.png)

Ens demanarà una nova contrasenya i posem una contrasenya provisional ja
que no deixarà posar la contrasenya patata per la política de
contrasenyes del mysql

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image22.png)

Posarem la comanda per veure les dues política de contrasenya que tenim
que canviar

![Escala de tiempo Descripción generada automáticamente con confianza
media](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image23.png)

Canviem la política de contrasenyes a low i li posem un length de 6 amb
això podrem posar la contrasenya 'patata'

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image24.png)

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image25.png)

I ara si podrem cambiar el password a "patata" amb aquesta comanda

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image26.png)

Ara farem les les instruccions per arrancar / verificar status / apagar
servei de la base de dades de Percona Server del sistema operatiu:

Per arrancar el mysql utilitzarem aquesta comanda

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image27.png)

I per apagar el mysql utilitzarem aquesta comanda

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image28.png)

Per verificar el estatus utilitzarem aquesta comanda

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image29.png)

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
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image30.png)

Crea un usuari anomenat asix en el sistema operatiu i en SGBD de tal
manera que aquest usuari del sistema operatiu no hagi d\'introduir
l\'usuari i password cada vegada que cridem al client mysql

Creem el usuari asix

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image31.png)

Quan intentem canviar la contrasenya ens diu que no podem, tenim que
tenir mínim 8 caràcters així que tindrem que canviar la política de
contrasenyes en el sistema operatiu.

![Interfaz de usuario gráfica, Texto, Sitio web Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image32.png)

Per canviar la política tenim que anar a la següent ruta

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image33.png)

I obrim el arxiu de configuració de la política de contrasenyes

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image34.png)

Busquem el apartat de la longitud de la contrasenya y ho canviem a 6 y
ho guardem

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image35.png)

I ara ja podem canviar la contrasenya a "patata"

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image36.png)

Creem el usuari asix amb la contrasenya patata dins del mySQL del root

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image37.png)

Per poder accedir al Mysql sense password del usuari Asix primer tindrem
que crear un arxiu de configuració en la ruta següent

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image38.png)

Y dins del fitxer de configuració posem el script de la contrasenya i ho
guardem

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image39.png)

Ja podem accedir al mysql del asix sense contrasenya:

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image40.png)

El servei de MySQL (mysqld) escolta al port 3306.

Els passos que faríem per canviar el port per defecte de mysql 3306 a
33306 son les següents:

Primer parem el servei de mysql

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image41.png)

I després anem a la ruta de configuració del percona.

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image42.png)

I si no hi ha port posem el port 33306 i ho guardem.

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image43.png)

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

# **[PART III -- INSTAL ·LACIÓ SGBD MongoDB]{.underline}**

En primer lloc, abans de la instal·lació del MongoDB, hem de crear un
repositori per tal de instal·lar el MongoDB, mitjançant el paquet yum,
per això editem el repositori situat a /etc/yum.repos.d/

![](./images//media/image57.png){width="5.625785214348206in"
height="0.20836286089238845in"}

![Texto Descripción generada
automáticamente](./images//media/image58.png){width="6.686805555555556in"
height="1.4270833333333333in"}

Una vegada fet això iniciem la instal·lació amb la següent comanda, que
el que fa es instal·lar la ultima versió del MongoDB:

![](./images//media/image59.png){width="4.344355861767279in"
height="0.20836286089238845in"}

Ara iniciem la base de dades, i seguidament amb el estatus, veiem com
esta el servei, en aquest cas actiu!

![Interfaz de usuario gráfica, Texto Descripción generada
automáticamente](./images//media/image60.png){width="6.686805555555556in"
height="4.029861111111111in"}

![](./images//media/image61.png){width="3.656760717410324in"
height="0.16668963254593175in"}

![Texto Descripción generada
automáticamente](./images//media/image62.png){width="6.686805555555556in"
height="3.092361111111111in"}

![Texto Descripción generada
automáticamente](./images//media/image63.png){width="5.407004593175853in"
height="2.239896106736658in"}

Webgrafia:

-   <https://docs.mongodb.com/v5.0/tutorial/install-mongodb-on-red-hat/>

-   <https://www.youtube.com/watch?v=NB-l3AeYxDg&ab_channel=Academind>

**[\
]{.underline}**

# **[PART IV -- INSTAL·LACIÓ SGBD Redis]{.underline}** 

Actualitzem els paquets del sistema juntament amb els repositoris
utilitzant la següent comanda: ![Texto Descripción generada
automáticamente](./images//media/image64.png){width="6.657179571303587in"
height="1.5835542432195975in"}

Seguidament executem la següent comanda per tal de instal·lar la ultima
versio de redis.:

![Texto Descripción generada
automáticamente](./images//media/image65.png){width="6.686805555555556in"
height="6.863194444444445in"}

Veiem la versió que disposem amb la següent comanda:

![](./images//media/image66.png){width="4.208920603674541in"
height="0.40630686789151355in"}

Ara una vegada aqui només ens faltaria activar i iniciar el servei el
servei de Redis i per tal ho fem amb la següent comanda:

![Una captura de pantalla de un celular Descripción generada
automáticamente con confianza
media](./images//media/image67.png){width="6.686805555555556in"
height="0.6965277777777777in"}Ara per veure que tot el que hem fet ja
sigui la instal·lació o iniciar el servei estigues ve, veiem si esta
actiu el servei i que no ens salti nungun error:

![Texto Descripción generada
automáticamente](./images//media/image68.png){width="6.686805555555556in"
height="3.0097222222222224in"}

Ara hem de configurar Redis per acces remot ja que

la instalación predeterminada només permet conexions desde el servidor
localhost i bloqueja qualsevol conexió externa, fer fer-ho accedim al
arxiu de configuració:

![Texto Descripción generada
automáticamente](./images//media/image69.png){width="6.686805555555556in"
height="5.615972222222222in"}

Substituim el parametre bind 127.0.0.1 per bind 0.0.0.0 per tal de
podernos connectar-nos exteriorament

![](./images//media/image70.png){width="1.1355752405949255in"
height="0.2604527559055118in"}

Ara hem de reiniciar el servei de redir per tal de que s'actualitzi el
que acabem de fer i per allo fiquem aquest comanda:

![](./images//media/image71.png){width="4.042230971128609in"
height="0.1875262467191601in"}

Ara iniciem i fem unping al servei de redis per veure si hi ha connexio:

![Imagen que contiene Texto Descripción generada
automáticamente](./images//media/image72.png){width="2.5211854768153983in"
height="0.5625787401574803in"}

Tal com es veu funciona ja que retorna el PONG (Ping-Pong)

Configuració de Firewall REDIS per tal de tenir una connexió remota amb
el servidor ja que predeterminadament no te el port 6379 obert:

![Texto, Escala de tiempo Descripción generada
automáticamente](./images//media/image73.png){width="5.834146981627296in"
height="0.6980139982502187in"}

Tal com es veu ens retorna un succes, que ens dona a entendre de que ho
ha fet correctament!Recarguem i ens torna a retorna de que esta bé. Ara
com a ultim pas hem de connectarnos al servidor amb el programa
redis-cli

![Texto Descripción generada
automáticamente](./images//media/image74.png){width="6.686805555555556in"
height="0.6972222222222222in"}

***Quin tipus de SGBD és Redis?** Redis utilitza la base de
dades **NoSQL** del tipus clau-valor **(key-value store)** distribuïda
en memòria **(in-memory database).***

Webgrafia:

-   <https://www.linuxtechi.com/install-redis-server-on-centos-8-rhel-8/>

-   <https://www.tecmint.com/install-redis-in-rhel-8/>

-   <https://linuxhint.com/install-redis-centos/>
