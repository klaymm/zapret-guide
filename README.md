# Zapret для Windows - Discord, YouTube, игры и сервисы

Это пошаговый гайд по сборке Flowseal. **Проверено по релизу 1.10.4 на 5 ноября 2026.** Тред [#8673](https://github.com/Flowseal/zapret-discord-youtube/discussions/8673) создал я ([klaymm](https://github.com/klaymm)). В исходном посте я отмечал, что гайд попадал в топ выдачи Google. Найти его можно по запросу "запрет гайд".

## Разделы

- [Быстрый старт](#быстрый-старт) - скачать, распаковать и подобрать стратегию.
- [Установка и настройки сети](docs/SETUP.md) - глобальная очистка, DNS, прокси, сброс сети и управление службой.
- [Решение проблем](docs/TROUBLESHOOTING.md) - ошибки запуска, YouTube, Discord, SoundCloud, Modrinth, RuTracker и WinDivert.
- [Игры и Steam](docs/GAMES.md) - Game Filter, IPSet, пользовательские списки и поиск доменов.
- [Telegram и hosts](docs/TELEGRAM.md) - обновление официального блока для Discord и Telegram Web, прокси для Telegram Desktop.
- [Антивирус и VirusTotal](docs/VIRUSTOTAL.md) - проверка происхождения архива, SHA-256 и детектов.
- [Полезные ссылки](docs/LINKS.md) - справка, инструменты и обсуждения с решениями.

> [!IMPORTANT]
> Скачивайте готовый архив с официальной страницы релизов. Выбирайте `zapret-discord-youtube-1.10.4.zip` или `.rar` в разделе Assets. Проверяйте, что владелец репозитория - Flowseal. [Последний релиз](https://github.com/Flowseal/zapret-discord-youtube/releases/latest) · [Предупреждение о поддельных сборках](https://github.com/Flowseal/zapret-discord-youtube/issues/1130)

## Быстрый старт

- [ ] **Подготовьте старую установку.** Если на ПК уже был zapret, GoodbyeDPI или другой обход, сначала пройдите [глобальную очистку](docs/SETUP.md#глобальная-очистка). Там же описано, как сохранить свои списки перед обновлением.
- [ ] **Скачайте и распакуйте релиз.** Скачайте ZIP из Assets официального релиза. В Проводнике нажмите правой кнопкой по архиву --> "Свойства" --> "Разблокировать" --> "Применить", если пункт есть. Затем нажмите правой кнопкой --> "Извлечь всё". Выберите короткий путь без кириллицы и спецсимволов, например `C:\zapret-1.10.4`. Откройте папку, где видны `service.bat`, `general.bat`, `bin`, `lists` и `utils`. При необходимости [сверьте SHA-256 ZIP](docs/VIRUSTOTAL.md#антивирус-и-virustotal).
- [ ] **Проверьте сеть и DNS.** Настройте [безопасный DNS](docs/SETUP.md#безопасный-dns). Для первой проверки используйте Chrome или Firefox. Если настраиваете Discord или Telegram Web, сразу добавьте [весь официальный блок hosts](docs/TELEGRAM.md#hosts-для-discord-и-telegram). Если раньше пользовались VPN или прокси, пройдите [проверку настроек сети](docs/SETUP.md#настройки-сети).
- [ ] **Подберите стратегию.** Дважды нажмите `service.bat` и подтвердите запрос Windows. Вводите номер пункта и нажимайте Enter. Если `3. Check Status` показывает установленную службу, запишите имя стратегии и выберите `2. Remove Services`. Запустите `12. Run Tests` --> `1. Standard tests (HTTP/ping)` --> `1. All configs`. Для проверки нескольких BAT выберите `2. Selected configs` и введите номера через запятую, например `1,3,5`. Дождитесь строки `Best config`.
- [ ] **Проверьте результат и настройте автозапуск при необходимости.** Дважды нажмите BAT из `Best config`. [Проверьте нужный сайт или приложение](docs/TROUBLESHOOTING.md#как-читать-результаты-теста). Для смены BAT сначала [остановите текущую стратегию](docs/SETUP.md#как-выключить-и-включить-zapret). Для автозапуска остановите ручную стратегию, откройте `service.bat` --> `1. Install Service` и введите номер нужного BAT из меню. В `3. Check Status` должны отображаться выбранная стратегия, запущенная служба `zapret` и `Bypass (winws.exe) is RUNNING`. [Меню 1.10.4](https://github.com/Flowseal/zapret-discord-youtube/blob/1.10.4/service.bat#L68-L112) · [Код тестов](https://github.com/Flowseal/zapret-discord-youtube/blob/1.10.4/utils/test%20zapret.ps1#L414-L446)

В 1.10.4 обновили IPSet, добавили TLS- и QUIC-фейки, поменяли основной TLS-фейк в ALT11, ALT12, EXP и SIMPLE FAKE ALT2, а в диагностике добавили обнаружение Happ. Отдельно 4 ноября в `main` обновили данные IPSet. В разделе [Игры и Steam](docs/GAMES.md#игры-и-steam) есть шаги, как обновить список и сохранить свои записи. [Релиз 1.10.4](https://github.com/Flowseal/zapret-discord-youtube/releases/tag/1.10.4) · [Обновление IPSet от 4 ноября](https://github.com/Flowseal/zapret-discord-youtube/pull/18572)
