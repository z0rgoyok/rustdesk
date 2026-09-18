# Share Desk X Plus

Управляемая Windows x64-сборка RustDesk `1.4.9` для собственного сервера.

## Встроенная конфигурация

- приложение: `Share Desk X Plus`;
- ID server: `share-desk-x-plus.tich.app`;
- relay server: выводится клиентом из того же hostname, стандартный порт
  `21117/tcp`;
- API server: отсутствует, используется RustDesk Server OSS;
- публичный ключ: фиксируется workflow в `libs/hbb_common/src/config.rs` перед
  сборкой.

Новое имя приложения создаёт отдельный Windows config namespace. Настройки
обычного RustDesk не переносятся в Share Desk X Plus.

## Поставка

`.github/workflows/flutter-build.yml` запускается вручную отдельными точными
редакциями для Windows x64 и macOS arm64. Результат включает portable EXE, MSI
или DMG, SHA-256 и GitHub build provenance attestations. Единый prerelease
`share-desk-x-plus-1.4.9.5` содержит Windows x64 и macOS arm64. macOS-сборка
имеет отдельные app name и bundle identifier `app.tich.share-desk-x-plus`.

Сборка не подписана Windows code-signing certificate. При первом запуске
Windows SmartScreen может запросить дополнительное подтверждение.
