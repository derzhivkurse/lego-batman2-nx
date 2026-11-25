# Установка LEGO Batman 2 на Nintendo Switch

[Скачать ZIP для microSD](https://github.com/derzhivkurse/lego-batman2-nx/releases/download/installer/lego-batman2-nx-sd.zip) · [Страница выпуска](https://github.com/derzhivkurse/lego-batman2-nx/releases/tag/installer) · [Поддержка в Telegram](https://t.me/derzhivkurse_games)

## Что понадобится

- Nintendo Switch с Atmosphère и Homebrew Menu. Для плитки в HOME нужен sys-patch.
- Свой диск LEGO Batman 2 для Xbox 360 (USA) или его ISO. Title ID `57520817`, Media ID `1BF17B45`.
- Около **4,45 ГБ** свободного места на microSD при копировании распакованных файлов или **13,2 ГБ** при установке из ISO, который лежит на той же карте. После запуска игра создаёт кэш.

## Установка с файлами своего диска

1. Распакуйте ZIP в корень microSD. Папка `switch` из архива должна оказаться в корне карты.
2. Извлеките файлы своего диска на компьютере и скопируйте в `/switch/lego-batman2-nx/game_root/` пять файлов из дерева ниже.
3. На Switch откройте **LB2 Installer** в Homebrew Menu в режиме приложения. Если используете title override, удерживайте **R** при запуске установленной игры до открытия Homebrew Menu.
4. Нажмите **A**. Когда установщик покажет `Ready`, запустите **LEGO Batman 2** из меню HOME.

Основные файлы на microSD перед запуском установщика

```text
sdmc:/
└── switch/
    ├── lb2-installer/
    │   └── lb2-installer.nro
    └── lego-batman2-nx/
        ├── lego-batman2-nx.nro
        ├── lego_batman2.toml
        └── game_root/
            ├── default.xex
            ├── GAME.DAT
            ├── GAME0.DAT
            ├── GAME1.DAT
            └── GAME2.DAT
```

В Homebrew Menu отображаются два приложения. **LB2 Installer** управляет установкой, **LEGO Batman 2** открывает игровой NRO. Для обычного запуска используйте плитку игры в HOME.

## Установка с ISO на SD

1. Распакуйте тот же ZIP в корень карты. Удалите `PUT_THE_DISC_FILES_HERE.txt` из `/switch/lego-batman2-nx/game_root/`. Для установки из ISO папка должна быть пустой.
2. Положите ISO в корень карты. На FAT32 заранее разделите большой образ на части по 2 ГБ с именами `Batman.iso.00`, `Batman.iso.01` и так далее.
3. Откройте **LB2 Installer** в режиме приложения и нажмите **A**. После `Ready` запустите игру из HOME. Копию образа с карты можно убрать после проверки запуска.

## Повтор, обновление и удаление

- После прерванной распаковки снова нажмите **A**. Установщик использует уже проверенные части.
- Для обновления плитки в HOME нажмите **X**, затем **Y**, затем **A**. Если после `Ready` видна старая обложка, перезапустите Switch.
- Для обновления игры закройте её и замените `lego-batman2-nx.nro`. Сохраните `game_root`, `lego_batman2.toml` и `userdata` на месте. Прежний NRO можно сохранить как резервную копию.
- Чтобы убрать только плитку, нажмите **X**, затем **Y**. Чтобы убрать плитку и файлы, которыми управляет установщик, нажмите **X**, затем **A**. Перед удалением можно скопировать сохранения из `/switch/lego-batman2-nx/userdata/`.

## Как включить логи

В игре нажмите **L + R + вправо на крестовине**. Откройте **Log**, затем **log_level** и выберите `info`. Если игра завершается до меню, выставьте `log_level = "info"` в `/switch/lego-batman2-nx/lego_batman2.toml` перед запуском. В игровом ZIP уровень `info` уже включён.

Опишите, что делали перед сбоем, и приложите журнал.

- Установка — `/switch/lego-batman2-nx/installer.log`.
- Игра — последний `/switch/lego-batman2-nx/logs/lego_batman2_*.log`.
- Сбой Atmosphère — код ошибки или соответствующий файл из `/atmosphere/crash_reports/`.

[Написать в Telegram](https://t.me/derzhivkurse_games)
