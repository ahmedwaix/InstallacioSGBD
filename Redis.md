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

***Quin tipus de SGBD és Redis?** Redis utilitza la base de
dades **NoSQL** del tipus clau-valor **(key-value store)** distribuïda
en memòria **(in-memory database).***

Webgrafia:

-   <https://www.linuxtechi.com/install-redis-server-on-centos-8-rhel-8/>

-   <https://www.tecmint.com/install-redis-in-rhel-8/>

-   <https://linuxhint.com/install-redis-centos/>
