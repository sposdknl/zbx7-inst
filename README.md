# Instalace Zabbix server 
Independent work - Zabbix server installation using Vagrant and automation

Samostatná práce - instalace Zabbix serveru pomocí Vagrant a automatizace

## Zadání: Instalace Zabbix serveru a agenta pomocí Vagrant

Úvod:
V tomto úkolu budete instalovat Zabbix server. Vaším cílem je nainstalovat Zabbix server i agenta. Máte možnost vybrat si mezi manuální instalací nebo automatizací procesu pomocí skriptů a nástrojů, což bude bodově zvýhodněno.

## 1. Příprava projektu

- Zprovozněte si svůj studentský repozitář na GitHub Classroom. Přidejte do repozitáře všechny soubory, které budete potřebovat (např. Vagrantfile, provisioning skripty, dokumentaci).

### Příprava prostředí

- Vytvořte Vagrantfile, který, vytvoří virtuální server přidejte je do repozitáře.
- Specifikuje základní parametry (např. RAM 2GB, počet CPU 2, síťové nastavení portforward 22 a 80).
- Linuxovou distribuci zvolte z examples. Ne Ubuntu !!!
- Pokud použijete provisioning nástroje (např. Bash, Ansible), přidejte je do repozitáře.

## 2. Instalace Zabbixu 7.0 LTS

### Vyberte jednu z možností:
- Manuální instalace (max. 10 bodů)
    Zabbix server ručně:
        Nainstalujte a nastavte webový server (např. Apache/Nginx).
        Nainstalujte databázi (např. MySQL/PostgreSQL) případně i s TimescaleDB
        Stáhněte a nainstalujte Zabbix server a jeho komponenty.
        Nakonfigurujte přístup na webové rozhraní.

    Zabbix agent2 ručně:
        Nainstalujte Zabbix agent2.
        Připojte agenta k serveru.

    Zaznamenejte všechny kroky instalace do dokumentace formou README.md
    Ověřte, že agent komunikuje se serverem a data jsou viditelná v Zabbix webovém rozhraní.

- Automatizovaná instalace (max. 30 bodů)

    Použijte provisioning nástroj (např. Ansible, Bash) pro automatizaci:
        Instalace a konfigurace Zabbix serveru.
        Instalace a konfigurace Zabbix agenta.

    Skripty přidejte do repozitáře a ověřte jejich funkčnost.
    Zaznamenejte všechny kroky instalace do dokumentace formou README.md
    Ověřte, že agent komunikuje se serverem a data jsou viditelná v Zabbix webovém rozhraní.

## 3. Monitoring
    Monitorujte SSL certifikát školního webu:
        Importujte Hosta
        Zkontrolujte, že se Certifikát https://sposdk.cz monitoruje (Latest data) případně screen obrazovky

## 4. Dokumentace
    V repozitáři vytvořte soubor README.md, kde popíšete:
        Postup instalace (pro manuální i automatizovanou variantu).
        Způsob spuštění virtuálních strojů pomocí Vagrantu.
        Jak ověřit funkčnost Zabbixu.

    Přiložte snímky obrazovky:
        Běh Zabbix serveru a agenta (logy, procesy, htop, ps, btop).
        Webové rozhraní Zabbixu. (Každý bude mít svůj Zabbix podepsaný) - $ZBX_SERVER_NAME v zabbix.conf.php
        Snímky budou součástí Vašeho repository adresář Images

## 5. Hodnocení

| Kritérium                     | Body |
|-------------------------------|------|
| Funkční Vagrantfile           | 5    |
| Manuální instalace serveru    | 5    |
| Manuální instalace agenta     | 1    |
| Automatizovaná instalace      | 10   |
| Monitoring SSL certifikátu    | 4    |
| Dokumentace                   | 5    |

## 6. Odevzdání
    Nahrajte svůj projekt do svého GitHub Classroom repozitáře.
    Zkontrolujte, že vše funguje podle zadání.
    Odevzdejte link na váš repozitář do Teams.
