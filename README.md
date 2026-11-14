# Viewmodel Lab — скачать игру

[Обновление 0.68: все версии](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/tag/0.68.0)

- [Windows x64 — ZIP](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/download/0.68.0/SpiralEngine-0.68-Windows-x64.zip)
- [Android ARM64 — APK](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/download/0.68.0/ViewmodelLab-0.68-arm64.apk)
- [iPhone / LiveContainer — IPA](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/download/0.68.0/ViewmodelLab-0.68.ipa)

Windows 10/11 x64, DirectX 11: распакуйте весь архив и запустите `SpiralEngine.exe`. Папки данных и UnityPlayer.dll должны оставаться рядом.

Android 8.0+, ARM64, OpenGL ES 3. Скачайте APK и разрешите установку из выбранного браузера или файлового менеджера. Подпись сохранена; приложение обновляется поверх прежней версии. Оставьте около 5 ГБ для установки и данных.

iOS 13.0+: IPA без подписи для импорта в LiveContainer. Источник LiveContainer ниже тоже обновлён до 0.68.

## Обновление 0.68

Оптимизированы проверки видимости: неподвижная камера больше не заставляет повторно обходить статичную карту. Двери, разрушение и восстановление объектов продолжают обновляться. В парном тесте Inferno 2000 проверок заняли 19 мс вместо 118 мс; это замер отдельного компонента, а не прирост FPS в шесть раз.

При загрузке статичные исходные меши больше не отправляются на GPU перед их объединением. Убраны лишние промежуточные загрузки. Пик памяти в тесте снизился; замеры выполнены в программном графическом окружении, не на realme.

Автографика теперь учитывает частоту экрана и доступную частоту вывода кадров. Она не пытается получить 120 FPS на экране 60 Гц за счёт ненужного снижения разрешения. Выбранные ограничения FPS сохраняются. Исправлена ошибка фильтрации текстур в настройках качества.

Проверены карты, двери и разрушения при неподвижной камере, отображение стен и скрытых агентов, фонтан, гранаты, попадания и восстановление графики. Нативный Direct3D 11 шейдер Windows проверен через Wine. Физический realme пока не проверен; FPS на устройстве не измерен.

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

Используются существующие аккаунты, друзья, комнаты, официальный подбор и напарники. Результаты рейтинговых матчей фиксирует сервер. Протокол 0.68 не изменён. Отдельные ведущие работают на текущем стенде; круглосуточная работа не гарантируется.

## Источник LiveContainer

`https://raw.githubusercontent.com/kokasikhorik-bot/viewmodel-lab-source/main/source.json`

LiveContainer → Источники → + → URL источника.

Каталог содержит только README, иконку и источник LiveContainer. Игровой код находится в отдельном закрытом репозитории. Для установки выбирайте APK, IPA или Windows ZIP из релиза.

Предыдущие сборки: [0.67 — все платформы](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/tag/0.67.0), [0.66 — все платформы](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/tag/0.66.0), [0.65 — все платформы](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/tag/0.65.0), [0.64 — все платформы](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/tag/0.64.0), [0.63 — все платформы](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/tag/0.63.0).

SHA-256 файлов: [SHA256SUMS.txt](https://github.com/kokasikhorik-bot/viewmodel-lab-source/releases/download/0.68.0/SHA256SUMS.txt).
