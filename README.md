# nginx-Konfiguration für OXID eShops

* Die Dateien aus diesem Repository in den nginx-Konfigurationsordner (`/etc/nginx/`) legen.
* Konfigurationsdatei (`oxid.conf`) anpassen
  * absoluten Pfad zum Web-Root-Verzeichnis angeben
    `root /var/www;`
* symlink im Ordner sites-enabled auf die Konfigurationsdatei aus dem Ordner sites-available erzeugen
  `ln -s /etc/nginx/sites-available/oxid.conf oxid.conf`
* nginx neu starten
  `service nginx restart`


Credits
Stefan Krenz @ Mayflower

Die Konfiguration ist aus folgendem Blogbeitrag entnommen: http://blog.mayflower.de/777-Nginx-Rewrite-Regeln-fuer-OXID-eShop-.html
