#INSTAL·LACIÓ MOODLE

A l'hora de fer l'instal·lació, hi hem de tenir una maquina amb LAMP (Linux, Apache, PHP y MySQL).

Un cop la tenim instal·lada, hi començem a ler l'instal·lació del apche. 
Abans de fer tot aixo per poder copiar del tutorial, ens unirem mijançant ssh a la MV a traves de la maquina real.

![](1uniossh.png)

Un cop feta la commanda, ens demanara la contrasenya i l'usuari per a poder accedir a la maquina de manera remota.

![](2queensdemana.png)

##INSTAL·LACIÓ APACHE

Ara el primer que hi farem hi es instal·lar el apache2.

![](3installapache.png)

Un cop ho tenim, ja estaria. Ara anirem a instal·lar MariaDB.

##INSTAL·LACIÓ MARIADB

El primer que hi farem es instal·lar la base de dades de mariaDB amb la seguent comanda.

![](4mariaDB.png)

Un cop finalitzat ejecutarem la configuracio del servidor de la base de dades.

![](5..securinstall.png)

I si un cop fet volem accedir a la base de dades ho podem fer amb la seguent comanda.

![](5.mariaDB.png)

Ara ja el que ens toca es instalar el php.

##INSTAL·LACIÓ DEL PHP

El primer que hi farem es instal·lar les propietats del software.

![](6php.png)

Un cop ho tenim, hi hem d'afegir el repositori.

![](6.1php7.3,1.png)

Despres i farem un update per afegir el repositori.

![](6.2php7.3,1.png)

I ja per ultim instal·larem la versió 7.3 del php.

![](6.3php7.3,1.png)

Un cop ho tenim, entrarem dins del seguent fitxer amb la seguent comanda.

![](6.4php7.3,1pref.png)

I a dins del fitcher i canviarem la preferencia a llocs acabats en php.

![](6.5php7.3,1 canvi.png)

Ara i reiniciarem i comprovarem l'estat d'apache2.

![](6.6php7.3,1restar.png)

Ara un cop finalitzat tot aixo i hem de anar a instal·lar la versio que necessitem del moodle.

##INSTAL·LACIÓ MOODLE

Per instal·lar el moodle, hi entrem a la seva pagina web dins de descargas i buscarem la versio que volem. hi entrarem i ademes de descargar el zip,
hi hem de copiar l'enllaç a la descarga.

![](7copiaenllaçDescarga.png)

Ara a dins la terminal hi afegirem la seguent commanda per descargar el zip.
Un cop ho tenim, hi tenim que descomprimir l'arxiu.

![](9descomprimirhtml.png)

Un cop fet, a la carpeta moodle li hem de canviar els permisos.

![](10canvipermisos)

Un cop fet, hi crearem una carpeta anomenada moodledata i li canviarem els permisos.

![](11crearmoodledata.png)

I ja abans de entrar al navegador i buscar per començar a configurar dins de la base de dades, i crearem un usuari amb la contrasenya.

![](12crearusuersialtres)

I ja un cop entrem al buscador, hi ens surtira aixo.

![](13començarconfiguracio.png)

El primer que ens demana es que li diguessim l'idioma que hi volem. En aquest cas en catala.

![](![image](https://user-images.githubusercontent.com/114162286/205091469-1cc10155-a2f9-4b7c-a919-dc3efa530918.png)

Al fer seguen, ens sortira aixo.

(![image](https://user-images.githubusercontent.com/114162286/205093338-26638d4d-600b-4bc8-a936-dec8b5e22182.png)


Per instal·lar el curl, ja que ja hi tenim els repositoris, podem sercar el curl. I intal·lar la versio pertinyent del php curl.

(![image](https://user-images.githubusercontent.com/114162286/205093179-36098097-83d1-4ee1-9727-3f378f9da98c.png)
