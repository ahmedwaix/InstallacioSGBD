**CFGS Administració de Sistemes Informàtics a la Xarxa**

**Mòdul 10:** Administració de sistemes gestors de base de dades (ASIX)

**UF 1:** Llenguatges SQL: DCL i extensió procedimental SGBD corporatiu


***


**Activitat 1: Instal·lació SGBD**


***

**Gaurav Pal**

**Ahmed Belhadi**

**ASIX**

**18/03/2022**
***

# **[ABANS DE LA INSTAL·LACIÓ]** 

1.  Primer abans de res, ens creem una copte d'usuari en la web de
    RedHat: <https://access.redhat.com/tags/login>
    ![Interfaz de usuario gráfica, Texto, Aplicación Descripción generada
    automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image1.png)

2.  Ara, iniciem la subscripció i activem la llicencia de 60 dies
    ![Interfaz de usuario gráfica, Texto, Aplicación Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image2.png)

3.  Esborrem la subscripció que havia tingut prèviament 
    ![Texto Descripción generada
    automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image3.png)

4.  Deixem de registrar-nos a l'antic compte

    ![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image4.png)

5.  Eliminem la suscrpció

    ![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image5.png)

6.  Ara fiquem el codi següent, per tal de connectar-se via consola:
    ![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image6.png)
    ![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image7.png)

***

# **[PART II - INSTAL·LACIÓ SGBD MySQL 8.0]** 

Per fer la instal·lació primer descarreguem el rpm del MYSQL

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image47.png)

Després instal·lem el rpm en dirà si volem acceptar i li donem que si

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image48.png)

Comprovem amb aquesta comanda si estan els repositoris

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image49.png)

Activem els repositoris y per això tindrem que desactivar els mòduls es
dirà si volem desactivar-lo i li diem que si![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image50.png)

Una vegada desactivat el mòdul ja podem instal·lar el MYSQL

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image51.png)

Ens dirà si volem instal·lar-lo i li donem que si

![Forma, Rectángulo Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image52.png)

Ens dirà si volem instal·lar les claus importades i li donem que si a
tot i amb això ja tindrem instal·lat el MYSQL

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image53.png)

**A on es troben físicament els fitxers de dades?** 
*Els fitxers de dades del MYSQL es troben a /var/lib/mysql/*

**A on es troba el fitxer de configuració? Quin és el seu contingut?**

*El fitxer de configuració del MySQL és troba en /etc/my.cnf. *

Per sabé el que conte el fitxer de configuració anem a aquesta ruta i modifiquem el
arxiu

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image54.png)

El que conté el fitxer de configuració són buffers i diverses rutes del
mysql.![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image55.png)

El procés de mysqld escolta al port 3306.

Els passos que faríem per canviar el port per defecte de MYSQL 3306 a
33306 son les següents:

Primer parem el servei de MYSQL

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

Un cop finalitzada la instal·lació i veure que funciona, mostra el
resultat de la comanda:

![Texto Descripción generada automáticamente con confianza
media](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image56.png)

***
Webgrafia:

-   *<https://computingforgeeks.com/how-to-install-percona-mysql-server-on-centos-rhel/#:~:text=%20Install%20Percona%20MySQL%20Server%208%20on%20CentOS,installation%20created%20a%20new%20repository%20file...%20More%20>*

-   *<https://www.linkedin.com/pulse/how-change-mysql-default-port-3306-secure-piyush-diwakar?msclkid=051592a2a53f11ecb903621e37f5ee4f>*

-   *<https://dev.mysql.com/doc/refman/8.0/en/installing.html>*

