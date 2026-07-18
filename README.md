# ⚡ ZAPRET: ПОЛНЫЙ ГАЙД
### Discord · YouTube · Игры · Сервисы

> **📌 Это официальная и актуальная версия гайда. Сохраните репозиторий в закладки (⭐ Star), чтобы всегда иметь к нему доступ — даже если сторонние площадки окажутся недоступны.**

> Если гайд оказался полезным — поставьте ⭐ **Star**: это помогает другим пользователям его найти.

---

## 📖 Содержание

Гайд разбит на разделы для удобной навигации:

| Раздел | Описание |
|---|---|
| **[🛠 Установка и настройка](docs/SETUP.md)** | Подготовка системы, очистка, сброс сети, установка (Этапы 0–3) |
| **[🎮 Игры и сервисы](docs/GAMES.md)** | Настройка сервисов, игр, ipset, списки доменов (Этапы 4–5) |
| **[🔧 Решение проблем](docs/TROUBLESHOOTING.md)** | Решения из сотен реальных случаев (Этап 6) |
| **[📨 Telegram](docs/TELEGRAM.md)** | Почему не работает и как ускорить (Этап 7) |
| **[🛡 VirusTotal и антивирусы](docs/VIRUSTOTAL.md)** | Почему детектится и что делать (Этап 8) |

---

> [!WARNING]
> ### 🔴 НЕ СКАЧИВАЙТЕ СТОРОННИЕ СБОРКИ
> Многочисленные «сборки запрета из Telegram/YouTube» содержат вредоносный код. Скачивайте **только** с официального репозитория [Flowseal/zapret-discord-youtube](https://github.com/Flowseal/zapret-discord-youtube/releases).

---

> [!CAUTION]
> ### ⚠️ Яндекс.Браузер и РУ-браузеры непригодны для тестов
>
> Благодарим [@V3nilla](https://github.com/V3nilla) и [@Dronatar](https://github.com/Dronatar) за обнаружение данной проблемы: [Issue #6083](https://github.com/Flowseal/zapret-discord-youtube/issues/6083).
>
> Начиная с октября 2025 года, российские браузеры (Яндекс.Браузер и им подобные) начали **принудительно подменять DNS** на собственные серверы (`77.88.8.8`) и блокировать любые сторонние DoH. Zapret при этом может работать идеально, но тесты в таком браузере всегда покажут отрицательный результат.
>
> ✅ Используйте для проверки: **Firefox, Brave, Chrome, Edge**

---

## 🔗 ПОЛЕЗНЫЕ ССЫЛКИ

<details>
<summary>📂 <b>Развернуть список ресурсов</b></summary>

### 🛠 Диагностика и анализ
| Инструмент | Описание |
|---|---|
| [wifiman.com](https://wifiman.com/) | Проверка скорости интернета |
| [Global Latency Test](https://github.com/hyperion-cs/dpi-checkers) | Обнаружение метода блокировки TCP 16–20 в РФ |
| [DNSCheck](https://dnscheck.tools/) | Проверка на утечку DNS, валидация |
| [IPList](https://iplist.opencck.org/ru) | Популярные домены и IP (CIDR) |
| [PingFast](https://pingfast.app/game-ports) | Порты и IP популярных игр |
| [Wireshark](https://www.wireshark.org/) | Глубокий анализ трафика |
| [Поиск доменов через Wireshark](https://wiki.malw.link/network/get-domains) | Инструкция по фильтрации доменов |
| [IP-Tracker](https://www.ip-tracker.org/) | Трекер IP-адресов |
| [Включение Secure DNS на Win 11](https://www.howtogeek.com/765940/how-to-enable-dns-over-https-on-windows-11/) | Гайд по DoH |

### 📺 Видео
- [«Как же на самом деле работает zapret?»](https://youtu.be/fOQ6vE6mpaw?si=E1D0nKXU9beLj6TZ)

### 📌 Треды с решениями (GitHub Issues & Discussions)
- **Discord:** [#252](https://github.com/Flowseal/zapret-discord-youtube/discussions/252), [#7873](https://github.com/Flowseal/zapret-discord-youtube/issues/7873), [#7899](https://github.com/Flowseal/zapret-discord-youtube/discussions/7899), [#12614](https://github.com/Flowseal/zapret-discord-youtube/issues/12614)
- **Discord + AdGuard (5000ms пинг / RTC):** [#13149](https://github.com/Flowseal/zapret-discord-youtube/issues/13149)
- **Discord: демонстрация экрана:** [#7921](https://github.com/Flowseal/zapret-discord-youtube/issues/7921), [#8511](https://github.com/Flowseal/zapret-discord-youtube/issues/8511), [#8773](https://github.com/Flowseal/zapret-discord-youtube/issues/8773), [#12495](https://github.com/Flowseal/zapret-discord-youtube/issues/12495)
- **Apex, Valorant:** [#7699](https://github.com/Flowseal/zapret-discord-youtube/issues/7699), [#7472](https://github.com/Flowseal/zapret-discord-youtube/issues/7472), [#7633](https://github.com/Flowseal/zapret-discord-youtube/issues/7633), [#7360](https://github.com/Flowseal/zapret-discord-youtube/issues/7360), [#8235](https://github.com/Flowseal/zapret-discord-youtube/issues/8235)
- **Ошибки батника / запуска:** [#7490](https://github.com/Flowseal/zapret-discord-youtube/issues/7490), [#7565](https://github.com/Flowseal/zapret-discord-youtube/issues/7565), [#522](https://github.com/Flowseal/zapret-discord-youtube/issues/522), [#7210](https://github.com/Flowseal/zapret-discord-youtube/issues/7210)
- **Loaded не меняется на Any:** [#6888](https://github.com/Flowseal/zapret-discord-youtube/issues/6888)
- **Telegram:** [#5820](https://github.com/Flowseal/zapret-discord-youtube/issues/5820)
- **Radmin VPN / TAP-адаптеры:** [#4201](https://github.com/Flowseal/zapret-discord-youtube/issues/4201), [#1826](https://github.com/Flowseal/zapret-discord-youtube/issues/1826)
- **Интернет пропадает после перезагрузки:** [#3797](https://github.com/Flowseal/zapret-discord-youtube/discussions/3797)
- **Play Market, MS Store:** [IP Ranges List](https://github.com/lord-alfred/ipranges/tree/main/microsoft)
- **Steam:** [#7328](https://github.com/Flowseal/zapret-discord-youtube/issues/7328)
- **EAC (Dead by Daylight и др.):** [#7179](https://github.com/Flowseal/zapret-discord-youtube/issues/7179), [#7224](https://github.com/Flowseal/zapret-discord-youtube/issues/7224), [#6786](https://github.com/Flowseal/zapret-discord-youtube/issues/6786)
- **Minecraft:** [#6453](https://github.com/Flowseal/zapret-discord-youtube/discussions/6453), [#5667](https://github.com/Flowseal/zapret-discord-youtube/discussions/5667)

</details>

---

## 🚦 БЫСТРЫЙ ЧЕКЛИСТ ПЕРЕД НАЧАЛОМ

Отмечайте пункты по порядку. Если пропустить хотя бы один — гайд может не помочь.

- [ ] Яндекс.Браузер закрыт; для тестов используется Chrome / Firefox / Edge
- [ ] Отключены все сторонние обходы (ByeDPI, GoodbyeDPI, Proxifier)
- [ ] Отключена фильтрация в AdGuard Desktop (или `winws.exe` и `Discord.exe` добавлены в исключения)
- [ ] В Антивирусах (Kaspersky, Dr.Web и др.) zapret добавлен в исключения
- [ ] Killer Control Center: «Bandwidth Control» отключён (только для ПК с Killer NIC)
- [ ] Папка запрета будет расположена по пути `C:\zapret` — без кириллицы и пробелов!

---

## 📝 ПРИМЕЧАНИЯ И ИСТОЧНИКИ

- Авторство оригинального инструмента: [bol-van/zapret](https://github.com/bol-van/zapret).
- Windows-сборка, на которую опирается гайд: [Flowseal/zapret-discord-youtube](https://github.com/Flowseal/zapret-discord-youtube)
- Обсуждение-первоисточник этого гайда: [Flowseal/zapret-discord-youtube · Discussion #8673](https://github.com/Flowseal/zapret-discord-youtube/discussions/8673)
- Альтернативная сборка: [zapret-win-bundle](https://github.com/bol-van/zapret-win-bundle)
- Ускорение Telegram Desktop: [tg-ws-proxy](https://github.com/Flowseal/tg-ws-proxy)

---

*Если Вы нашли рабочее решение — поделитесь им в разделе Issues или Discussions, это поможет другим пользователям.*
