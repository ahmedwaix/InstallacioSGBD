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
