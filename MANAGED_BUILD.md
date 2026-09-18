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

`.github/workflows/flutter-build.yml` запускается вручную и собирает только
Windows x64 Flutter client. Результат включает portable EXE, MSI, `SHA256SUMS`
и GitHub build provenance attestations. Артефакты публикуются как Actions
artifact и prerelease `share-desk-x-plus-1.4.9.2`.

Сборка не подписана Windows code-signing certificate. При первом запуске
Windows SmartScreen может запросить дополнительное подтверждение.
