# Viewmodel Lab — скачать игру

[Обновление 0.67: все версии](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/tag/0.67.0)

- [Windows x64 — ZIP](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/download/0.67.0/SpiralEngine-0.67-Windows-x64.zip)
- [Android ARM64 — APK](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/download/0.67.0/ViewmodelLab-0.67-arm64.apk)
- [iPhone / LiveContainer — IPA](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/download/0.67.0/ViewmodelLab-0.67.ipa)

Windows 10/11 x64, DirectX 11: распакуйте весь архив и запустите `SpiralEngine.exe`. Папки данных и UnityPlayer.dll должны оставаться рядом.

Android 8.0+, ARM64, OpenGL ES 3. Скачайте APK и разрешите установку из выбранного браузера или файлового менеджера. Подпись сохранена; приложение обновляется поверх прежней версии. Оставьте около 5 ГБ для установки и данных.

iOS 13.0+: IPA без подписи для импорта в LiveContainer. Источник LiveContainer ниже тоже обновлён до 0.67.

## Обновление 0.67

Исправлена возможная причина ровно 30 FPS: команда fps_max 0 и сохранённое значение «без ограничения» больше не передают мобильной Unity значение -1 (платформенный стандарт, часто 30 FPS). Теперь запрашивается положительная частота экрана; добавлен выбор 90 FPS. Настройки 30/60 FPS и неограниченный FPS на ПК сохранены.

Оптимизированы карты и автоматическое качество на телефонах. Число поверхностей отрисовки всей карты снижено: Dust II — на 34,6%, Mirage — на 24,4%, Inferno — на 36,3%, Seaside — на 16,9%. Близкие статичные поверхности объединены с сохранением исходной видимости Source, дверей, прозрачной воды, освещения и общих теней карты/игроков. Материалы 3D-неба теперь переиспользуются. Убраны повторные обращения к состоянию неподвижных рендереров. Память объединённых мешей освобождается при выгрузке карты.

На телефоне в автоматическом высоком качестве: до 900p для 3D вместо 1080p, MSAA до 2×, две близко сфокусированные каскадные тени с прежним атласом 2048. HUD остаётся в разрешении экрана. Ручные настройки и настройки ПК доступны. Автоматическая адаптация включается в настройках изображения; для проверки оставьте лимит 60 FPS и включите счётчик FPS.

Проверены все четыре карты, сохранение геометрии и исходных PVS-индексов, интерактивные части, движущееся 3D-небо, освобождение мешей, фонтан Inferno и боевые проверки. Проверка стен с анимированным игроком за ними пройдена, включая телефонный режим и нативный Direct3D 11 шейдер Windows через Wine. Физический realme/Snapdragon 8 Gen 3 здесь не доступен: FPS на устройстве не измерен.

Windows: распакуйте весь ZIP и запустите SpiralEngine.exe. Android: APK 8.0+, ARM64, подпись сохранена — обновляется поверх прежней версии. iOS: IPA 13.0+ без подписи для LiveContainer.

Новости: https://t.me/SpiralEngine


## Заставка Spiral

Все три варианта из 0.64 сохранены: Настройки → Игра → Заставка Spiral.

- [1 — Проявление спирали](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/download/0.64.0/Spiral-intro-1.mp4)
- [2 — Световой проход](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/download/0.64.0/Spiral-intro-2.mp4)
- [3 — Сборка из дуг](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/download/0.64.0/Spiral-intro-3.mp4)

## Управление

Tab — таблица счёта; ПКМ по игроку — карточка. На телефоне нажмите строку игрока. B — выбор оружия; в дезматче он бесплатный. F2 — бонусное оружие. ~ / F1 — офлайн-консоль. Настройки → Управление — клавиши и мышь; Настройки → HUD — цвет интерфейса. В консоли: `help`, `find radar`, `cl_radar_scale 0.7`, `bind mouse4 +jump`.

## Онлайн

Используются существующие аккаунты, друзья, комнаты, официальный подбор и напарники. Результаты рейтинговых матчей фиксирует сервер. Протокол 0.67 не изменён. Отдельные ведущие работают на текущем стенде; круглосуточная работа не гарантируется.

## Источник LiveContainer

`https://raw.githubusercontent.com/kokasikhorik-bot/viewmodel-lab-source/main/source.json`

LiveContainer → Источники → + → URL источника.

Каталог содержит только README, иконку и источник LiveContainer. Игровой код находится в отдельном закрытом репозитории. Для установки выбирайте APK, IPA или Windows ZIP из релиза.

Предыдущие сборки: [0.66 — все платформы](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/tag/0.66.0), [0.65 — все платформы](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/tag/0.65.0), [0.64 — все платформы](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/tag/0.64.0), [0.63 — все платформы](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/tag/0.63.0).

SHA-256 файлов: [SHA256SUMS.txt](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/download/0.67.0/SHA256SUMS.txt).
