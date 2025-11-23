


# сохранение .config
make savedefconfig

# стандартная настройка ядра
make menuconfig

# пересборка линукс ядра
make linux-rebuild

# конфиг ядра линукс
make linux-menuconfig


# ПОЛНАЯ пересборка системы
make clean;make


#


#


# просто запуск
make


# настройка для qemu_//-//-
make qemu_x86_64_defconfig


    make menuconfig — вызвать настройку сборки. Так же можно с использование графического интерфейса (make nconfig,make xconfig,make gconfig)
    make linux-menuconfig — вызвать конфигурацию ядра.
    make clean — очистить результаты сборки (всё что храниться в output)
    make — собрать систему. При этом не выполняется пересборка уже собранных процессов
    make defconfig_name — переключить конфигурацию на определенный defconfig
    make list-defconfigs — показать список defconfig’ов
    make source — только скачать установочный файлы, без сборки.
    make help — вывести список возможных команд

    
    make graph-depends построить дерево зависимостей
    make <pkg>-graph-depends построить дерево зависимостей конкретного пакета
    BR2_GRAPH_OUT=png make graph-build построить график времени сборки с выводом в PNG
    make graph-size построить график размера пакетов



