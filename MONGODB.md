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

# **[PART III -- INSTAL ·LACIÓ SGBD MongoDB]{.underline}**

En primer lloc, abans de la instal·lació del MongoDB, hem de crear un
repositori per tal de instal·lar el MongoDB, mitjançant el paquet yum,
per això editem el repositori situat a /etc/yum.repos.d/

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image57.png)

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image58.png)

Una vegada fet això iniciem la instal·lació amb la següent comanda, que
el que fa es instal·lar la ultima versió del MongoDB:

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image59.png)

Ara iniciem la base de dades, i seguidament amb el estatus, veiem com
esta el servei, en aquest cas actiu!

![Interfaz de usuario gráfica, Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image60.png)

![](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image61.png)

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image62.png)

![Texto Descripción generada
automáticamente](https://github.com/ahmedwaix/InstallacioSGBD/blob/main/Imagenes/image63.png)

Webgrafia:

-   <https://docs.mongodb.com/v5.0/tutorial/install-mongodb-on-red-hat/>

-   <https://www.youtube.com/watch?v=NB-l3AeYxDg&ab_channel=Academind>

**[\
]{.underline}**
