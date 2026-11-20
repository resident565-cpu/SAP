# Ширина поля чтения статей на ПК — 20.11.2026

Основа: specagropartner-footer-caption-fix-2026-11-20.zip (файлы синхронизированы без изменений).
Изменён только assets/sap-glass.css (+5–7 % к ширине текста статей на ПК):

- .container-narrow: max-width 900px → 960px (+6,7 %)
- .article-card .article-body: max-width 72ch → 76ch (+5,5 %)
- .container-article: max-width 1320px → 1380px
- @media (min-width:1200px) .article-layout: grid-template-columns minmax(0,min(900px,calc(100% - 312px))) 280px → minmax(0,min(960px,calc(100% - 312px))) 280px
- @media (min-width:1200px) .article-layout>.article-card: max-width 900px → 960px

Проверено в браузере на 1280, 1440 и 1920 px: колонка статьи стала шире примерно на 60 px, боковая панель 280 px на месте, горизонтальной прокрутки нет.
Мобильная и планшетная вёрстка не менялась (правила для ширины до 1200 px не затронуты, кроме общего max-width контейнера, который на узких экранах не достигается).
