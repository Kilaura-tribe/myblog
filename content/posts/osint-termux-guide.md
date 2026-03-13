+++
date = '2026-03-13T17:32:07Z'
draft = false
title = 'OSINT в кармане: Установка Sherlock и Blackbird в Termux'
+++
---
title: "OSINT в кармане: Установка Sherlock и Blackbird в Termux"
date: 2026-03-13
draft: false
tags: ["OSINT", "Termux", "Sherlock", "Blackbird"]
---

Поиск информации о человеке по никнейму — одна из базовых задач в OSINT. Для этого не обязательно иметь ПК с Kali Linux, достаточно смартфона с Android и установленным Termux.

### Подготовка системы
Перед установкой инструментов обновим пакеты и установим Python с Git:

```
bash
pkg update && pkg upgrade
pkg install python git rust binutils
```

:Установка Sherlock:

​*Sherlock* ищет аккаунты по никнейму на более чем 400 сайтах.
 
1. Клонируем репозиторий:
```
git clone https://github.com/sherlock-project/sherlock.git
cd sherlock
```


2. Устанавливаем зависимости:
```
python3 -m pip install -r requirements.txt
```



3. Запуск:
```
python3 sherlock имя_пользователя
```



:Установка Blackbir:

*​Blackbird* — отличная альтернатива, которая часто находит то, что пропускает Sherlock.
 
1. Клонируем репозиторий:
```
git clone https://github.com/p1ngul1n0/blackbird
cd blackbird
```


2. Устанавливаем зависимости:
```
pip install -r requirements.txt
```


3. Запуск поиска:
Для запуска используйте команду с флагом -u (username):
```
python3 blackbird.py -u имя_пользователя
```


