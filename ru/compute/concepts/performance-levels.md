# Уровни производительности vCPU

Уровень производительности vCPU необходимо выбирать при создании каждой виртуальной машины. Уровень определяет гарантированную долю vCPU, которая будет выделена виртуальной машине. В зависимости от выбранной [платформы](vm-platforms.md) доступные конфигурации вычислительных ресурсов для разных уровней могут меняться.

- Виртуальные машины с гарантированной долей vCPU меньше 100% работают с частичным использованием ядра и предназначены для запуска приложений, не требующих высокой производительности. При этом такие машины обойдутся дешевле.
- Виртуальные машины с гарантированной долей vCPU 100% работают с полным использованием ядра и предназначены для запуска приложений, требующих высокой производительности.

Доступный объем диска не зависит от уровня производительности виртуальной машины. Ограничения приведены в разделе [[!TITLE]](limits.md).

Минимальные и максимальные конфигурации:

- Платформа Intel Broadwell:

    Конфигурация | vCPU | RAM, ГБ
    --- | --- | --- | ---
    Мин. | 1 | 1
    Макс. | 32 | 256

- Платформа Intel Cascade Lake:

    Конфигурация | vCPU | RAM, ГБ
    --- | --- | --- | ---
    Мин. | 2 | 0.5
    Макс. | 48 | 384

Доступные конфигурации вычислительных ресурсов:

- Платформа Intel Broadwell:

    Уровень</br> производительности | vCPU | RAM на 1 ядро, ГБ
    --- | --- | ---
    5% | 1, 2, 4 | 0.5, 1, 1.5, 2
    20% | 1, 2, 4 | 0.5, 1, 1.5, 2, 2.5, 3, 3.5, 4
    100% | 1, 2, 4, 6, 8, 10, 12,</br> 14, 16, 18, 20, 22, 24,</br> 26, 28, 30, 32 | 1, 2, 3, 4, 5, 6, 7, 8

- Платформа Intel Cascade Lake:

    Уровень</br> производительности | vCPU | RAM на 1 ядро, ГБ
    --- | --- | ---
    5% | 2, 4 | 0.25, 0.5, 1, 1.5, 2
    20% | 2, 4 | 0.5, 1, 1.5, 2, 2.5, 3, 3.5, 4
    50% | 2, 4 | 0.5, 1, 1.5, 2, 2.5, 3, 3.5, 4
    100% | 2, 4, 6, 8, 10, 12, 14,</br> 16, 20, 24, 28, 32, 36,</br> 40, 44, 48 | 1, 2, 3, 4, 5, 6, 7, 8