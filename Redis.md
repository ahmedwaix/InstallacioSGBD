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

# **[PART IV - INSTAL·LACIÓ SGBD Redis]** ![Interfaz de usuario gráfica, Texto, Aplicación Descripción generada     automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/redis.png)

Actualitzem els paquets del sistema juntament amb els repositoris
utilitzant la següent comanda: ![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image64.png)

Seguidament executem la següent comanda per tal de instal·lar la ultima
versio de redis.:

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image65.png)

Veiem la versió que disposem amb la següent comanda:

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image66.png)

Ara una vegada aqui només ens faltaria activar i iniciar el servei el
servei de Redis i per tal ho fem amb la següent comanda:

![Una captura de pantalla de un celular Descripción generada
automáticamente con confianza
media](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image67.png)
Ara per veure que tot el que hem fet ja
sigui la instal·lació o iniciar el servei estigues ve, veiem si esta
actiu el servei i que no ens salti nungun error:

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image68.png)

Ara hem de configurar Redis per acces remot ja que

la instalación predeterminada només permet conexions desde el servidor
localhost i bloqueja qualsevol conexió externa, fer fer-ho accedim al
arxiu de configuració:

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image69.png)

Substituim el parametre bind 127.0.0.1 per bind 0.0.0.0 per tal de
podernos connectar-nos exteriorament

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image70.png)

Ara hem de reiniciar el servei de redis per tal de que s'actualitzi el
que acabem de fer i per allo fiquem aquest comanda:

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image71.png)

Ara iniciem i fem un ping al servei de redis per veure si hi ha connexio:

![Imagen que contiene Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image72.png)

Tal com es veu funciona ja que retorna el PONG (Ping-Pong)

Configuració de Firewall REDIS per tal de tenir una connexió remota amb
el servidor ja que predeterminadament no te el port 6379 obert:

![Texto, Escala de tiempo Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image73.png)

Tal com es veu ens retorna un succes, que ens dona a entendre de que ho
ha fet correctament!Recarguem i ens torna a retorna de que esta bé. Ara
com a ultim pas hem de connectarnos al servidor amb el programa
redis-cli

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image74.png)

**Quin tipus de SGBD és Redis?** 

*Redis utilitza la base de
dades **NoSQL** del tipus clau-valor **(key-value store)** distribuïda
en memòria **(in-memory database).***

***

Webgrafia:

-   *<https://www.linuxtechi.com/install-redis-server-on-centos-8-rhel-8/>*

-   *<https://www.tecmint.com/install-redis-in-rhel-8/>*

-   *<https://linuxhint.com/install-redis-centos/>*
