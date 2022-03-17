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

# **[PART I -- INSTAL·LACIÓ SGBD MySQL Percona Server]{.underline}** 

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
