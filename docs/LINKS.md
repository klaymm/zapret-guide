# Ссылки и источники

[Оглавление](../README.md)

Подборка из [обсуждения #8673](https://github.com/Flowseal/zapret-discord-youtube/discussions/8673).

## Полезные ссылки

### Инструменты и справка

| Если нужно | Куда перейти |
| --- | --- |
| Найти старую папку zapret | Откройте Everything и введите `general.bat` или имя старой папки. Сверьте путь перед удалением. [Everything](https://www.voidtools.com/) |
| Сравнить скорость или DNS | В WiFiman запустите тест до и после изменения. В DNSCheck посмотрите обнаруженный DNS-резолвер. [WiFiman](https://wifiman.com/) · [DNSCheck](https://dnscheck.tools/) |
| Проверить признаки фильтрации | Откройте описание тестов и сравните с результатом `12. Run Tests` --> `2. DPI checkers`. [DPI checkers](https://github.com/hyperion-cs/dpi-checkers) |
| Найти хосты, IP и порты | Начните с [запросов браузера](GAMES.md#как-найти-домен-у-которого-сбой). Для сетевого анализа откройте Wireshark и инструкцию по поиску доменов. Справочники IP и портов используйте для сверки того, что увидели у себя. [Wireshark](https://www.wireshark.org/) · [Поиск доменов в Wireshark](https://wiki.malw.link/network/get-domains) · [IPList](https://iplist.opencck.org/ru/) · [PingFast](https://pingfast.app/game-ports) |
| Настроить безопасный DNS | Сверьте шаги под вашу систему или браузер. [Windows 11](https://support.microsoft.com/en-gb/windows/experience/connectivity-networking/essential-network-settings-and-tasks-in-windows) · [Яндекс Браузер](https://browser.yandex.ru/help/ru/security/dnscrypt) · [Chrome](https://support.google.com/chrome/answer/10468685) · [Firefox](https://support.mozilla.org/en-US/kb/dns-over-https) |
| Проверить, нет ли сбоя самого сервиса | Откройте страницу статуса и посмотрите, отмечен ли сбой в нужном компоненте. [Статус Discord](https://discordstatus.com/) · [Статус GitHub](https://www.githubstatus.com/) |
| Проверить файл по хэшу | Вставьте SHA-256 в `Search`. Сравните точный файл и названия детектов. [VirusTotal](https://www.virustotal.com/gui/home/search) · [Отчёты VirusTotal](https://docs.virustotal.com/docs/results-reports) |
| Понять общий принцип работы обходов | Видео из исходной подборки объясняет, как работают GoodbyeDPI и zapret. За номерами меню и настройками 1.10.4 обращайтесь к быстрому старту выше. [Видео Ильи Рублёва](https://www.youtube.com/watch?v=fOQ6vE6mpaw) |

### Обсуждения

- **Большие ветки по двум основным сервисам.** Начинайте с новых ответов, где совпадают ваш провайдер, версия и симптом. [Обход YouTube #251](https://github.com/Flowseal/zapret-discord-youtube/discussions/251) · [Обход Discord #252](https://github.com/Flowseal/zapret-discord-youtube/discussions/252)
- **Как исследуют сетевые проблемы.** В #3423 есть материалы по DNS и поиску доменов, IP и портов игры. В #3279 интересно посмотреть, как менялись стратегии и откуда вырос один из старых ALT. Совместимость пользовательских батников проверяйте отдельно. [Подборка #3423](https://github.com/Flowseal/zapret-discord-youtube/discussions/3423) · [История стратегий Dronatar #3279](https://github.com/Flowseal/zapret-discord-youtube/discussions/3279) · [DPI checkers](https://github.com/hyperion-cs/dpi-checkers)
- **Minecraft.** В одной ветке обсуждают серверы Hypixel и Minemen, в другой - конкретно Essential и e4mc. У них разные симптомы и разные точки отказа. [Серверы Minecraft #6453](https://github.com/Flowseal/zapret-discord-youtube/discussions/6453) · [Essential и e4mc #5585](https://github.com/Flowseal/zapret-discord-youtube/discussions/5585)
- **Roblox.** Для картинок и аватарок есть отдельная ветка. В комментариях видно, что IP из первого сообщения подошёл не всем. Отдельно есть большая ветка с доменами и экспериментами по клиенту. [Картинки и аватарки #16296](https://github.com/Flowseal/zapret-discord-youtube/discussions/16296) · [ROBLOX ZAPRET #6800](https://github.com/Flowseal/zapret-discord-youtube/discussions/6800)
- **Роутеры.** Для установки на роутер ищите инструкции по конкретной модели и прошивке в документации оригинального zapret. Шаги с `service.bat` выше относятся к Windows. [Вопрос про Keenetic #18610](https://github.com/Flowseal/zapret-discord-youtube/discussions/18610) · [Оригинальный zapret](https://github.com/bol-van/zapret)
- **Другие сервисы.** В ветках про TikTok и Imgur собраны пользовательские эксперименты с DNS и `hosts`. Читайте ответы после первого сообщения, поскольку старый IP может перестать отвечать. Если сервис сам ограничивает доступ по региону, добавление его домена в список zapret не меняет ваш внешний IP. [TikTok #18077](https://github.com/Flowseal/zapret-discord-youtube/discussions/18077) · [Imgur #18313](https://github.com/Flowseal/zapret-discord-youtube/discussions/18313) · [Пример с ChatGPT #18591](https://github.com/Flowseal/zapret-discord-youtube/issues/18591)

## Источники

Оригинальный инструмент разработал [bol-van](https://github.com/bol-van/zapret). Сборка под Windows и её релизы - [Flowseal/zapret-discord-youtube](https://github.com/Flowseal/zapret-discord-youtube). Альтернативная Windows-сборка автора оригинала - [zapret-win-bundle](https://github.com/bol-van/zapret-win-bundle).
