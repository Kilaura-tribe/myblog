+++
date = '2026-03-11T12:31:46Z'
draft = false
title = 'Установка nexfil в Termux'
+++
### Что такое nexfil?
**nexfil** — это крайне быстрый инструмент для поиска профилей по никнейму. В отличие от многих аналогов, он проверяет сотни сайтов за считанные секунды.
### Пошаговая установка:
1. **Обновляем систему:**
bash
   pkg update && pkg upgrade
2. Устанавливаем необходимые зависимости (Python и Git):

   pkg install python git
3. Клонируем репозиторий nexfil:
  
   git clone [https://github.com/thewhiteh4t/nexfil.git](https://github.com/thewhiteh4t/nexfil.git)
4. Переходим в папку и устанавливаем библиотеки:
  
    cd nexfil
    pip install -r requirements.txt
5. Запуск инструмента:
   Для поиска используйте команду: 
    python3 nexfil.py -u никнейм

