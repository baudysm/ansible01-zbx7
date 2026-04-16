# postup

Tady je ve zkratce postup, jak jsem to nastavil a rozchodil.

## 1. Příprava a sítě
Nejdřív jsem musel pořešit síťovku ve virtuálu, aby se to vůbec spojilo s labem. Udělal jsem si u toho screenshot, ať mám co dát do dokumentace. Pak jsem si stáhl kód z GitHubu a doinstaloval nějaký věci pro Ansible, co tam chyběly.

## 2. Oprava a instalace
Ten stažený soubor na instalaci byl rozbitý, takže jsem tam musel ručně dopsat chybějící části, aby to Ansible vůbec pobral. Nastavil jsem tam správný názvy, IP adresy a metadata. Pak jsem to pustil a ono si to samo nainstalovalo Zabbix Agenta i ty další balíčky (get a sender) a hned to i spustilo.

## 3. Kontrola
Když to dojelo, tak jsem si jen checknul, jestli to fakt funguje:
* Koukl jsem na status služby, jestli běží.
* Ověřil jsem si verzi (7.0).
* Zkontroloval jsem přes porty, jestli to naslouchá tam, kde má.

