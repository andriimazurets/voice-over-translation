# Закадровый перевод видео

[![en](https://img.shields.io/badge/lang-English%20%F0%9F%87%AC%F0%9F%87%A7-white)](README-EN.md)
[![ru](https://img.shields.io/badge/%D1%8F%D0%B7%D1%8B%D0%BA-%D0%A0%D1%83%D1%81%D1%81%D0%BA%D0%B8%D0%B9%20%F0%9F%87%B7%F0%9F%87%BA-white)](README.md)

Закадровый перевод видео, теперь, доступен не только в YandexBrowser.
Очень признателен, **[Yandex.Translate](https://translate.yandex.ru/)** & **[sodapng](https://github.com/sodapng)** & **[mynovelhost](https://github.com/mynovelhost)** & **[SashaXser](https://github.com/SashaXser)**. Спасиб <3

> [!NOTE]
> На 04.11.2023 большая часть языков доступных для выбора в качестве озвучки были отключены на стороне Яндекса. Мне неизвестно будут ли они возвращены позднее или нет. Из тех, на которые точно можно выполнить перевод остались: `Русский`, `Английский`, `Казахский`.

## Установка расширения:
1. Установите расширение **[Tampermonkey](https://www.tampermonkey.net/)** (Альтернатива для Safari: **[UserScripts](https://apps.apple.com/app/userscripts/id1463298887 )**)
   * ![image](https://github.com/andriimazurets/voice-over-translation/assets/127737896/ccba1c53-55b8-4dd4-ae96-bc0363042a43)
   * ![image](https://github.com/andriimazurets/voice-over-translation/assets/127737896/6660ac80-1a78-4353-bc5c-659fa26d5527)
3. **[«Установите Скрипт»](https://raw.githubusercontent.com/ilyhalight/voice-over-translation/master/dist/vot.user.js)** (**[Cloudflare version](https://raw.githubusercontent.com/ilyhalight/voice-over-translation/master/dist/vot-cloudflare.user.js)**)

### Полезные ссылки:
1. Версия для VioletMonkey, FireMonkey, GreaseMonkey, AdGuard, OrangeMonkey, UserScripts и некоторых браузеров: **[Ссылка](https://raw.githubusercontent.com/ilyhalight/voice-over-translation/master/dist/vot-cloudflare.user.js)**
2. Версия для терминала: **[Ссылка](https://github.com/FOSWLY/vot-cli)**
3. Вики: **[Link](https://github.com/ilyhalight/voice-over-translation/wiki)**

## Список поддерживаемых сайтов:
Все ограничения, связанные с поддержкой сайтов вы можете увидеть в [вики](https://github.com/ilyhalight/voice-over-translation/wiki/%5BRU%5D-Supported-sites).
- **[YouTube](https://www.youtube.com)**
- **[Twitch](https://www.twitch.tv)**
- **[VK](https://vk.com)**
- **[Twitter](https://twitter.com/)**
- **[9GAG](https://9gag.com/gag/)**
- **[Rutube](https://rutube.ru/)**
- **[Bilibili](https://bilibili.com/)**
- **[Видео Mail.ru](https://my.mail.ru/video)**
- **[Vimeo](https://vimeo.com/)**
- **[XVideos](https://xvideos.com/)**
- **[PornHub](https://rt.pornhub.com/)**
- **[Bitchute](https://www.bitchute.com/)**
- **[Coursera](https://www.coursera.org/)**
- **[[⚠️] Udemy](https://www.udemy.com/)**
- **[[❌] Facebook*](https://facebook.com/)**
- **[TikTok](https://tiktok.com/)**
- **[ProxiTok](https://proxitok.pabloferreiro.es/)**
- **[Invidious](https://yewtu.be)**
- **[Piped](https://piped.video)**

⚠️ - Требует дополнительных действий, подробнее в **[Wiki](https://github.com/ilyhalight/voice-over-translation/wiki)**

❌ - Не работает

## Список функционала:
1. Перевод с одного из доступных языков на русский. Язык определяется автоматически, если языка нету в списке или не удалось его определить, то используется перевод с английского.
2. Перевод с русского на английский язык
3. Автоматический перевод видео при открытие
4. Слайдер для изменения громкости видео
5. Автоматически выставлять громкость видео (как в Яндекс браузере)
6. [YouTube Only] Синхронизация громкости перевода с громкостью видео
7. [YouTube Only] Ограничить перевод русскоязычных видео

## Как собрать расширение?
1. Установите NodeJS 18+
2. Установите зависимости:
```bash
npm i
```
3. Сборка расширения:

   3.0. Все версии сразу:
   ```bash
   npm run build
   ```

   3.1. Все минифицированные версии сразу:
   ```bash
   npm run build:min
   ```

   3.2. Только обычная версии:
   ```bash
   npm run build:default
   ```

   3.3. Только Cloudflare версии:
   ```bash
   npm run build:cloudflare
   ```

   3.2. Только обычная мин. версии:
   ```bash
   npm run build:default-min
   ```

   3.3. Только мин. Cloudflare версии:
   ```bash
   npm run build:cloudflare-min
   ```


## Как задеплоить свой Cloudflare Worker?
[Нажми, чтобы перейти](https://github.com/ilyhalight/voice-over-translation/wiki/%5BRU%5D-Deploy-Cloudflare-Worker)

## Примечание:
1. Рекомендую разрешить автовоспроизведение "аудио и видео", чтобы избежать ошибок при работе расширения
2. Расширение не может переводить видео длиной более 4 часов (ограничение API переводчика)

## Расширение протестировано в следующих браузерах:
| Статус | Браузер | Версия браузера | Платформа | Расширение
|---|---|---|---|---
| ⠀✅ | Firefox Developer Edition | v106 — v117, 64 bit | Windows | Tampermonkey
| ⠀✅ | Firefox | v116.0.2 | Windows, Linux, Android | Tampermonkey, Violetmonkey
| ⠀✅ | Firefox Nightly | v118.0a1 | Windows, Android | Tampermonkey
| ⠀✅ | LibreWolf | v100.0.2-1 | Windows | Tampermonkey
| ⠀✅ | Brave | v106.0.5249.91 | Windows | Tampermonkey
| ⠀✅ | MS Edge | v106.0.1370.34 | Windows, Linux | Tampermonkey
| ⠀✅ | Cent Browser | v4.3.9.248, 32 bit | Windows | Tampermonkey
| ⠀✅ | Cent Browser Beta | v5.0.1002.182, 64 bit | Windows | Tampermonkey
| ⠀✅ | Google Chrome | v106 — 116 | Windows, MacOS, Linux | Tampermonkey, Violetmonkey, OrangeMonkey
| ⠀✅ | Opera GX | LVL4 (core: 91.0.4516.36) | Windows | Tampermonkey
| ⠀✅ | Opera | v92.0.4561.43 | Windows | Tampermonkey
| ⠀✅ | Vivaldi | 5.7.2921.63 | Windows, Linux | Tampermonkey
| ⠀❔ | Safari | v15.6.1 | MacOS, iOS | Userscripts
| ⠀✅ | Kiwi Browser | v116.0.5845.61 | Android | Tampermonkey

## Протестировано в следующих расширениях для юзерскриптов:
| Статус | Браузер | Расширение
|---|---|---
| ⠀✅ | Любой | Tampermonkey
| ⠀[Загрузить](https://raw.githubusercontent.com/ilyhalight/voice-over-translation/master/dist/vot-cloudflare.user.js) | Safari | Userscripts
| ⠀[Загрузить](https://raw.githubusercontent.com/ilyhalight/voice-over-translation/master/dist/vot-cloudflare.user.js) | Любой | Violetmonkey
| ⠀[Загрузить](https://raw.githubusercontent.com/ilyhalight/voice-over-translation/master/dist/vot-cloudflare.user.js) | Любой | [AdGuard Usercripts](https://kb.adguard.com/en/general/userscripts#supported-apps)
| ⠀[Загрузить](https://raw.githubusercontent.com/ilyhalight/voice-over-translation/master/dist/vot-cloudflare.user.js) | Firefox | Firemonkey
| ⠀[Загрузить](https://raw.githubusercontent.com/ilyhalight/voice-over-translation/master/dist/vot-cloudflare.user.js) | Любой | Greasemonkey
| ⠀[Загрузить](https://raw.githubusercontent.com/ilyhalight/voice-over-translation/master/dist/vot-cloudflare.user.js) | Любой | OrangeMonkey

![example btn](https://github.com/ilyhalight/voice-over-translation/blob/master/img/example.jpg "btn")

*: Запрещена на территории РФ
