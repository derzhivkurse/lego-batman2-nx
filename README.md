<h1 align="center">LEGO Batman 2 for Nintendo Switch</h1>

<p align="center">
  <strong>Рекомпиляция LEGO Batman 2: DC Super Heroes с Xbox 360 для Nintendo Switch</strong>
</p>

<p align="center">
  <a href="https://github.com/derzhivkurse/lego-batman2-nx/releases/download/installer/lego-batman2-nx-sd.zip"><img alt="Скачать ZIP для microSD" src="https://img.shields.io/badge/microSD-%D0%A1%D0%BA%D0%B0%D1%87%D0%B0%D1%82%D1%8C%20ZIP-F5BF37?style=for-the-badge"></a>
  <a href="https://t.me/derzhivkurse_games"><img alt="Поддержка в Telegram" src="https://img.shields.io/badge/Telegram-%D0%9F%D0%BE%D0%B4%D0%B4%D0%B5%D1%80%D0%B6%D0%BA%D0%B0-229ED9?style=for-the-badge&amp;logo=telegram&amp;logoColor=white"></a>
</p>

<p align="center">
  <a href="#о-порте">О порте</a> · <a href="#установка">Установка</a> · <a href="#поддержка">Поддержка</a> · <a href="https://github.com/derzhivkurse/lego-batman2-nx/releases/tag/installer">Страница выпуска</a>
</p>

---

## О порте

Код PowerPC из версии для Xbox 360 перекомпилирован для ARM64 и работает на Switch нативно. В ZIP уже есть игровой NRO, профиль 720p и **LB2 Installer**, который добавляет плитку игры в меню HOME. Подсказки в игре используют обозначения кнопок Switch.

Запуск с плитки HOME и игра проверены на Switch Lite на штатных частотах. В тяжёлых сценах Готэма возможны просадки частоты кадров.

> [!IMPORTANT]
> Для запуска нужны файлы **своего диска LEGO Batman 2 для Xbox 360 (USA)**. Поддерживаемое издание имеет Title ID `57520817` и Media ID `1BF17B45`.

## Установка

Понадобится Switch с **Atmosphère**, **Homebrew Menu** и **sys-patch** для плитки в HOME. Игра, установщик и файлы диска занимают около **4,45 ГБ** на microSD до создания кэша.

1. Скачайте [ZIP для microSD](https://github.com/derzhivkurse/lego-batman2-nx/releases/download/installer/lego-batman2-nx-sd.zip) и распакуйте его в корень карты.
2. Извлеките из своего диска или его ISO файлы `default.xex`, `GAME.DAT`, `GAME0.DAT`, `GAME1.DAT` и `GAME2.DAT`. Скопируйте их в `/switch/lego-batman2-nx/game_root/`.
3. Откройте **LB2 Installer** в Homebrew Menu в режиме приложения. Нажмите **A** и дождитесь `Ready`.
4. Запустите **LEGO Batman 2** из HOME.

Дерево папок, установка напрямую из ISO на карте, обновление и удаление описаны в [полной инструкции](INSTALL.md).

## Поддержка

По ошибкам и вопросам пишите в [Telegram](https://t.me/derzhivkurse_games). Укажите модель Switch, версию Atmosphère и шаги перед сбоем. Для установки приложите `installer.log`, для игры — свежий `logs/lego_batman2_*.log`. [Как включить и найти логи](INSTALL.md#как-включить-логи)

Там же публикуем обновления порта.
