CodeIgniter-Htaccess
====================

Htaccess soubor pro PHP framework **CodeIgniter**.

Požadavky
---------

* Web server Apache
* Framevork CodeIgniter


Obsahuje
--------

* Ochranu některých souborů před přímým zobrazením v prohlížeči (log, sql, ini, atd.)
* Zákaz procházení adresářů v prohlížeči
* Nastavení výchozího souboru
* Kontrolu zda je aktivní "mod_rewrite"
* Pravidla pro "hezká URL"
* Zákaz pro přístup do některých systémových složek CodeIgniteru
* Aktivaci "mod_deflate" pokud je k dispozici pro kompresi a tak rychlejší načítání stránek
* Nastavení "mod_expires" pokud je k dispozici pro rychlejší načítání stránek

Upozornění
----------

Pokud CodeIgniter provozujete v podsložce (například `www/blog/`), musíte htaccess soubor mírně upravit:
Řádek

```
RewriteBase /
```
musíte přepsat na

```
RewriteBase /blog/
```
viz. [htaccess a RewriteBase](https://www.google.com/search?q=htaccess+rewritebase)
