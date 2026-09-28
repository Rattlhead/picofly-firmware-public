# Data0Lab artifacts

В этом каталоге допускаются только проверенные `clean-install` UF2, созданные
исправленным конвейером. Наличие конкретной версии смотрите по её подпапке.

Предыдущие файлы удалены: прежний `clean-install` содержал RAM-образ `usk.bin`
без загрузчика, а двухслотовый `console-updater` несовместим с BY25Q20AW.

Новые файлы разрешено создавать только через `firmware-lab/build.sh`. Сборка
применяет односекционный загрузчик, создаёт полный USB/BOOTSEL `clean-install`
и перед публикацией проверяет структуру UF2, адреса, размер и CRC прошивки.

Техник-диагностический профиль 2.99 выпускается как
`PicoFly-2.99-led-context-diagnostics-clean-install.uf2`. Он устанавливается
только через USB/BOOTSEL, не содержит console updater, трассу или flash-журнал.

| Файл | Размер | SHA-256 |
| --- | ---: | --- |
| `PicoFly-2.99-led-context-diagnostics/PicoFly-2.99-led-context-diagnostics-clean-install.uf2` | 247296 байт | `154375bad92eccd111edc39b9999a767fbe4444bdc5510f11542947c03c14c3c` |
