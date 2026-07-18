# 🎮 ИГРЫ И СЕРВИСЫ

[← Назад к оглавлению](../README.md)

> 🔄 После любых изменений в списках: `service.bat` → **2 (Remove)** → **1 (Install)**

Все файлы списков находятся в `C:\zapret\lists\`.

---

## ЭТАП 4: НАСТРОЙКА СЕРВИСОВ И ИГР

### 4.1 — Файл `list-general-user.txt`

Добавьте сюда домены необходимых сервисов:

<details>
<summary>📄 <b>Показать содержимое list-general-user.txt</b></summary>

```text
; Instagram
static.cdninstagram.com
instagram.feed.com
cdninstagram.com
instagram.com
fbcdn.net
fbsbx.com

; Facebook
facebook.com
fbcdn.net
fbsbx.com
accountkit.com
facebookauth.com
facebook.net
fb.com
fb.me

; Twitter / X
x.com
api.x.com
twitter.com
api.tweetdeck.com
abs.twimg.com
pbs.twimg.com
video.twimg.com
t.co
abs-0.twimg.com

; Genshin Impact (Asia & Europe)
asia.genshin.mihoyo.com
hk4e-api.mihoyo.com
api-takumi.mihoyo.com
download.genshin.mihoyo.com
genshin.hoyoverse.com
hk4e-api-os.mihoyo.com
hk4e-sdk-os.mihoyo.com
log-upload-os.mihoyo.com
dispatchosglobal.mihoyo.com
osasiadispatch.mihoyo.com
oseurodispatch.mihoyo.com
webstatic-sea.mihoyo.com
minor-api-os.hoyoverse.com
sg-public-data-api.hoyoverse.com
log-upload-os.hoyoverse.com
sentry.eks.hoyoverse.com

; Arc Raiders
privacy.xboxlive.com
api.epicgames.dev
api-gateway.europe.es-pio.net
client2pubsub.europe.es-pio.net
es-pio.net
es-cf.net

; Speedtest
speedtest.net

; Modrinth
modrinth.com

; Rutracker
rutracker.org
static.rutracker.cc
fastpic.org

; SoundCloud
soundcloud.cloud
soundcloud.com
sndcdn.com

; Essential (Minecraft мод)
essential.gg
imagedelivery.net
```

</details>

### 4.2 — Фикс Nvidia App

Если Nvidia App не загружается, добавьте в системный hosts (`C:\Windows\System32\drivers\etc\hosts`):

```
185.246.223.127 developer.nvidia.com
```

---

## ЭТАП 5: НАСТРОЙКА IPSET

1. Откройте `C:\zapret\lists\ipset-all.txt`
2. Убедитесь, что в настройках запрета установлено значение `Switch ipset: loaded`

### Genshin Impact & Arc Raiders

<details>
<summary>📄 <b>Показать IP-адреса для ipset-all.txt</b></summary>

```text
; Genshin Impact (Asia & Europe)
47.91.24.239
116.251.83.218
47.100.0.0/15
47.102.0.0/15
47.116.0.0/17
43.132.28.160
43.132.29.187
43.132.31.114
43.132.28.122
43.132.29.164
43.132.31.45

; Arc Raiders
34.4.16.0/20
34.4.32.0/19
34.4.64.0/19
34.4.96.0/22
34.4.128.0/18
34.6.0.0/15
34.8.0.0/13
34.16.0.0/12
34.32.0.0/11
34.64.0.0/10
34.128.0.0/10
35.184.0.0/13
35.192.0.0/14
35.196.0.0/15
35.198.0.0/16
35.199.0.0/17
35.199.128.0/18
35.200.0.0/13
35.208.0.0/12
35.224.0.0/12
35.240.0.0/13
136.107.0.0/16
136.108.0.0/14
136.112.0.0/13
```

</details>

---

[← Назад к оглавлению](../README.md) · [Далее: Решение проблем →](TROUBLESHOOTING.md)
