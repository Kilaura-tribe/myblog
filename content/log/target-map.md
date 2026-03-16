---
title: "Карта связей: Объект Passenger_01"
date: 2026-03-16
categories: ["investigation"]
---

Визуализация цифрового следа.

### Схема связей:

{{< mermaid >}}
graph TD
    Target((Passenger_01)) --> Email[mail@example.com]
    Target --> Phone[+380...]
    Email --> Facebook[FB Profile]
    Email --> Instagram[IG Profile]
    Phone --> Telegram[TG Account]
    Telegram --> Group1((BlackHat Chat))
    Facebook --> Job[Company Name]
{{< /mermaid >}}

> Данная схема построена на основе открытых данных.
