# Viewmodel Lab — скачать игру

[Обновление 0.66: все версии](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/tag/0.66.0)

- [Windows x64 — ZIP](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/download/0.66.0/SpiralEngine-0.66-Windows-x64.zip)
- [Android ARM64 — APK](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/download/0.66.0/ViewmodelLab-0.66-arm64.apk)
- [iPhone / LiveContainer — IPA](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/download/0.66.0/ViewmodelLab-0.66.ipa)

Windows 10/11 x64, DirectX 11: распакуйте весь архив и запустите `SpiralEngine.exe`. Папки данных и UnityPlayer.dll должны оставаться рядом.

Android 8.0+, ARM64, OpenGL ES 3. Скачайте APK и разрешите установку из выбранного браузера или файлового менеджера. Подпись сохранена; приложение обновляется поверх прежней версии. Оставьте около 5 ГБ для установки и данных.

iOS 13.0+: IPA без подписи для импорта в LiveContainer. Источник LiveContainer ниже тоже обновлён до 0.66.

## Обновление 0.66

Исправлены ложные контуры и полосы на стенах при приближении и наклонном взгляде. Исправление 0.65 не закрывало этот случай в полном игровом кадре.

Контактное затенение теперь использует точную аппаратную глубину и нормали той же видимой поверхности. Убрана потеря точности упакованной линейной глубины. Параметры глубины берутся у камеры мира, отдельно от камеры оружия и финального изображения. Видимое контактное затенение и динамические тени сохранены; лишний проход нормалей больше не запрашивается. Дополнительная камера или повторный рендер сцены не добавлены.

Проверен реальный кадр Dust II с игроком, камерой оружия, финальным композитом и динамическим солнцем: обе стороны освещения, обычное/полное качество затенения, скрытый агент в покое и беге, видимый агент и выступ перед стеной как контроль. Та же проверка выявляет ошибку в рендерере 0.65. Проверены 1560×720 и телефонный режим 1280×590 с масштабом 75% и MSAA 2×; нативный шейдер Windows проверен через Wine/DirectX 11 с неотгружаемым тестовым модулем. Архивы всех трёх платформ проверены по содержимому, шейдерам и контрольным суммам. Физические Android/iPhone и FPS на RTX 4060 здесь не измерялись.

Windows: распакуйте весь ZIP и откройте SpiralEngine.exe. Android: APK 8.0+, ARM64; подпись сохранена, можно обновить поверх предыдущей версии. iOS: IPA 13.0+ без подписи для LiveContainer.

Новости: https://t.me/SpiralEngine


## Заставка Spiral

Все три варианта из 0.64 сохранены: Настройки → Игра → Заставка Spiral.

- [1 — Проявление спирали](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/download/0.64.0/Spiral-intro-1.mp4)
- [2 — Световой проход](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/download/0.64.0/Spiral-intro-2.mp4)
- [3 — Сборка из дуг](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/download/0.64.0/Spiral-intro-3.mp4)

## Управление

Tab — таблица счёта; ПКМ по игроку — карточка. На телефоне нажмите строку игрока. B — выбор оружия; в дезматче он бесплатный. F2 — бонусное оружие. ~ / F1 — офлайн-консоль. Настройки → Управление — клавиши и мышь; Настройки → HUD — цвет интерфейса. В консоли: `help`, `find radar`, `cl_radar_scale 0.7`, `bind mouse4 +jump`.

## Онлайн

Используются существующие аккаунты, друзья, комнаты, официальный подбор и напарники. Результаты рейтинговых матчей фиксирует сервер. Протокол 0.66 не изменён. Отдельные ведущие работают на текущем стенде; круглосуточная работа не гарантируется.

## Источник LiveContainer

`https://raw.githubusercontent.com/kokasikhorik-bot/viewmodel-lab-source/main/source.json`

LiveContainer → Источники → + → URL источника.

Каталог содержит только README, иконку и источник LiveContainer. Игровой код находится в отдельном закрытом репозитории. Для установки выбирайте APK, IPA или Windows ZIP из релиза.

Предыдущие сборки: [0.65 — все платформы](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/tag/0.65.0), [0.64 — все платформы](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/tag/0.64.0), [0.63 — все платформы](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/tag/0.63.0).

SHA-256 файлов: [SHA256SUMS.txt](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/download/0.66.0/SHA256SUMS.txt).
