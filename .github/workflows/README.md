# GitHub Actions workflows

CI/CD-рецепты управляемого fork RustDesk. Windows workflow выпускает
проверяемый Share Desk X Plus x64 client из закреплённого исходного дерева.

## Файлы

| Файл | Назначение и связи | Версия содержимого |
| --- | --- | --- |
| [bridge.yml](./bridge.yml) | Требует ручного описания назначения, существенных входов, выходов и связей. | a7b74fa55a1c0f2b1acac8c7514a11758ea205d3 |
| [ci.yml](./ci.yml) | Требует ручного описания назначения, существенных входов, выходов и связей. | 173eda9f456fdb6e48dd705b84d17c9438b53deb |
| [clear-cache.yml](./clear-cache.yml) | Требует ручного описания назначения, существенных входов, выходов и связей. | 0a1af9e6f5fddb88136551986d299890abf23211 |
| [fdroid.yml](./fdroid.yml) | Требует ручного описания назначения, существенных входов, выходов и связей. | db3767b113a7c93e67fb8f09ee53b10ad4984cc0 |
| [flutter-build.yml](./flutter-build.yml) | Собирает Windows x64 portable EXE и MSI; после checkout детерминированно задаёт имя Share Desk X Plus, `share-desk-x-plus.tich.app` и публичный ключ, создаёт SHA-256, attestations, Actions artifact и prerelease. | 77c8155c036c927b3cfdd5c14afe93dffc62bed6 |
| [flutter-ci.yml](./flutter-ci.yml) | Требует ручного описания назначения, существенных входов, выходов и связей. | a64dd11972a659c3721dcbf07076085c4de5ebe9 |
| [flutter-nightly.yml](./flutter-nightly.yml) | Требует ручного описания назначения, существенных входов, выходов и связей. | b16db4c4a6a17a47bd8c12cd0ba21c5c6c11ee2a |
| [flutter-tag.yml](./flutter-tag.yml) | Требует ручного описания назначения, существенных входов, выходов и связей. | bf39db5ccee81bbb540cc8a50b2cca3e857415d3 |
| [playground.yml](./playground.yml) | Требует ручного описания назначения, существенных входов, выходов и связей. | 41b9c0c139fb072aebe1eead968864dca1ac3b50 |
| [third-party-RustDeskTempTopMostWindow.yml](./third-party-RustDeskTempTopMostWindow.yml) | Требует ручного описания назначения, существенных входов, выходов и связей. | 05c8731d5e5769edd3d94ebf14a2fc69b2804123 |
| [wf-cliprdr-ci.yml](./wf-cliprdr-ci.yml) | Требует ручного описания назначения, существенных входов, выходов и связей. | bc65d22e8663be6dfa847f2d5f0786994580d7d6 |
| [README.md](./README.md) | Карта содержимого и правила работы с папкой. | — (самоописание) |

## Подпапки

| Папка | Назначение |
| --- | --- |
| — | Непосредственных подпапок нет. |

## Работа с папкой

Перечень и версии содержимого сверяет `.agents/skills/folder-readme/scripts/sync_folder_readmes.py`.

Последняя полная сверка перечня и версий содержимого: 2026-09-18T10:00:49.979514000Z.
