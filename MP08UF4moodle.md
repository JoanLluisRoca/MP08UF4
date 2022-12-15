# INSTAL·LACIÓ MOODLE

A l'hora de fer l'instal·lació, hi hem de tenir una maquina amb LAMP (Linux, Apache, PHP y MySQL).

Un cop la tenim instal·lada, hi començem a ler l'instal·lació del apche. 
Abans de fer tot aixo per poder copiar del tutorial, ens unirem mijançant ssh a la MV a traves de la maquina real.

![](1uniossh.png)

Un cop feta la commanda, ens demanara la contrasenya i l'usuari per a poder accedir a la maquina de manera remota.

![](2queensdemana.png)

## INSTAL·LACIÓ APACHE

Ara el primer que hi farem hi es instal·lar el apache2.

![](3installapache.png)

Un cop ho tenim, ja estaria. Ara anirem a instal·lar MariaDB.

## INSTAL·LACIÓ MARIADB

El primer que hi farem es instal·lar la base de dades de mariaDB amb la seguent comanda.

![](4mariaDB.png)

Un cop finalitzat ejecutarem la configuracio del servidor de la base de dades.

![](5..securinstall.png)

I si un cop fet volem accedir a la base de dades ho podem fer amb la seguent comanda.

![](5.mariaDB.png)

Ara ja el que ens toca es instalar el php.

## INSTAL·LACIÓ DEL PHP

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

## INSTAL·LACIÓ MOODLE

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

![image](https://user-images.githubusercontent.com/114162286/205091469-1cc10155-a2f9-4b7c-a919-dc3efa530918.png)

Al fer seguen, ens sortira aixo.

![image](https://user-images.githubusercontent.com/114162286/205093338-26638d4d-600b-4bc8-a936-dec8b5e22182.png)

Per instal·lar el curl, ja que ja hi tenim els repositoris, podem sercar el curl. I intal·lar la versio pertinyent del php curl.

![image](https://user-images.githubusercontent.com/114162286/205093179-36098097-83d1-4ee1-9727-3f378f9da98c.png)

I ara hem de instalar lo zip pertinyent.

![image](https://user-images.githubusercontent.com/114162286/205094084-97e9650f-a349-4aa4-94f0-6b766d6d7428.png)

Un cop ho tenim hi reiniciem el apache2.

![image](https://user-images.githubusercontent.com/114162286/205094522-7b303033-ba84-434f-adee-11ec9faee0cc.png)

El seguent que ens demana es la URL de moodle, el directori de moodle i el directori de dades de l'usuari.

![image](https://user-images.githubusercontent.com/114162286/205095422-fe5f4800-191d-4544-8d69-e18bd916cb81.png)

Un cop posat tot ens demanara qun controlador de base de dades utilitzarem.

![image](https://user-images.githubusercontent.com/114162286/205095905-4dbe6990-3c6c-4ae8-acd3-8cbb6be86b59.png)

Ara el que ens prefuntara es la direccio de la base de dades, el nom de la base de dades i l'usuari i la contrasenya.

![image](https://user-images.githubusercontent.com/114162286/205096548-2d99d651-54d4-4a1b-bf75-66d7e7c4ab4d.png)

Ara al fer seguent, hi he trobat un error.

![image](https://user-images.githubusercontent.com/114162286/205097337-c11f967f-e1b1-4a5a-8889-e7c30a5ca053.png)

Per resoldre aixo, anirem a la terminal de la maquina hi farem la seguent comanda.

![image](https://user-images.githubusercontent.com/114162286/205099312-d2745402-7be7-435b-928f-28d45c87bcf3.png)

Per seguir, tindriem que entrar dins del seguent fitxer hi fer els seguent tal com apl fitxer.

![image](https://user-images.githubusercontent.com/114162286/205100004-e51573da-e077-412b-939b-ce83f97cf21c.png)

Un cop dins i fem un restart.

![image](https://user-images.githubusercontent.com/114162286/205100341-ce032d91-1662-4fe3-8d7b-dca9694a058a.png)

Ara ens demana que intalesem un paquet.El cual es el seguent.

![image](https://user-images.githubusercontent.com/114162286/205100681-b12ccf90-7ea3-49e9-a604-f805ac9ee016.png)

Per resoldre aixo farem la seguent comanda.

![image](https://user-images.githubusercontent.com/114162286/205101146-434bb3ac-5f5f-4c89-90bf-366bbe77fc07.png)

Ara resetegem el apache2.

![image](https://user-images.githubusercontent.com/114162286/205101488-25433ad7-cf70-4a26-9714-9986d90a2fe4.png)

Ara ens demanara que intalaresem una altra cosa, el cual es el seguent.

![image](https://user-images.githubusercontent.com/114162286/205102200-0cc298c1-a060-464d-a8b0-69b5f3bb9e0e.png)

Aixi que en la seguent comanda.

![image](https://user-images.githubusercontent.com/114162286/205102645-5518b9e0-104f-44ad-89c0-7357ab5904cf.png)

I fem el reload.

![image](https://user-images.githubusercontent.com/114162286/205101488-25433ad7-cf70-4a26-9714-9986d90a2fe4.png)

Ara ja hem surt que s'ha intalat amb exit.

![image](https://user-images.githubusercontent.com/114162286/205102978-af425b45-6f90-4099-85c5-20e4351c7735.png)

Ara ens sortira una pantalla per a que intalesim i revisesim el seguent.

![image](https://user-images.githubusercontent.com/114162286/205103479-e26d3ced-954d-4ba3-9fa2-38db043b65e9.png)

Ho farem amb la seguent comanda.

![image](https://user-images.githubusercontent.com/114162286/205104322-f126052a-b60e-48b2-881d-bd493aa50861.png)

I farem un reload al apache2.

![image](https://user-images.githubusercontent.com/114162286/205101488-25433ad7-cf70-4a26-9714-9986d90a2fe4.png)

I ens quedara aixi i porem continuar.

![image](https://user-images.githubusercontent.com/114162286/205104858-6c4f7560-d96a-449d-8ece-2283d095d641.png)

Continuem i ens sortira aixo.

![image](https://user-images.githubusercontent.com/114162286/205107472-46d3d176-5605-4138-8d2c-c5c37d071c6d.png)

Un cop continuem aurem de posar una contrasenya.

![image](https://user-images.githubusercontent.com/114162286/205109438-911f6018-893d-4b17-8129-d02b4a2367d7.png)

Un cop ho tenim hem de configurar la pagina de moodle en tituls i descripcions.

![image](https://user-images.githubusercontent.com/114162286/205110421-d0e8fad7-7a5f-408b-ad87-1a438c62975d.png)

I per ultim ja tindrem aixo.

![image](https://user-images.githubusercontent.com/114162286/205110826-e71c895d-a041-4aaf-9726-c4791d91b438.png)
