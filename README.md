# MyApp - System Information Utility / Утилита информации о системе

**English** | [Русский](#русский)

## English

**MyApp** - a command-line utility for displaying system information, similar to the popular **neofetch** program, but written in Python.

### 🌟 Features

- 📋 Display OS and Linux distribution information
- 🔧 Linux kernel version information
- 💻 CPU details (model and number of cores)
- 🧠 RAM size
- 💾 Disk space usage
- ⏱️ System uptime
- 🐚 Current shell and user
- 🕐 Current date and time
- 🌐 **Bilingual support** - English and Russian

### 🚀 Quick Start

#### Option 1: Install from .deb package (recommended)

```bash
sudo dpkg -i myapp_1.0.0_all.deb
```

#### Option 2: Build and install with script

```bash
chmod +x build-and-install.sh
./build-and-install.sh
```

#### Option 3: Install from source

```bash
cd myapp
sudo python3 setup.py install
```

#### Option 4: Install with pip

```bash
cd myapp
pip install -e .
```

### 📖 Usage

```bash
# Show info in system language (or English by default)
myapp

# Show info in Russian
myapp ru

# Show info in English
myapp en

# Show help
myapp --help
```

## 📤 Example Output

```
    ╔═══════════════════╗
    ║    MyApp Info     ║
    ╚═══════════════════╝

User..................... user@ubuntu
OS....................... Ubuntu 24.04.3 LTS
Kernel................... 6.8.0-1012-generic
CPU...................... Intel(R) Core(TM) i7-9700K (8 cores)
RAM...................... 16Gi
Disk..................... 50G / 100G
Uptime................... 5d 3h 42m
Shell.................... bash
Time..................... 2025-12-07 14:23:15
```

### 📁 Project Structure

```
myapp/
├── myapp/                      # Python package
│   ├── __init__.py             # Package initialization
│   └── main.py                 # Main module with SystemInfo class
├── debian/                     # Files for .deb packaging
│   ├── control                 # Package metadata
│   ├── rules                   # Build rules
│   ├── changelog               # Change history
│   ├── copyright               # License information
│   ├── compat                  # Debhelper version
│   └── source/format           # Source format
├── setup.py                    # Setup tools configuration
├── README.md                   # This file
└── build-and-install.sh        # Installation script
```

### 🔧 Requirements

- Python 3.6+
- Linux (Ubuntu, Debian, Fedora, etc.)
- Access to `/etc/os-release`, `/proc/cpuinfo`, `/proc/uptime`

### 📦 Uninstall

```bash
sudo apt remove myapp
# or
sudo dpkg -r myapp
```

### 📝 License

MIT License - see `debian/copyright` for details.

### 👥 Author

MyApp Team ylolvideo@gmail.com

---

# Русский

**MyApp** - утилита командной строки для отображения информации о системе, аналогичная популярной программе **neofetch**, но написанная на Python.

## 🌟 Возможности

- 📋 Отображение информации об ОС и дистрибутиве Linux
- 🔧 Информация о версии ядра
- 💻 Сведения о процессоре (модель и количество ядер)
- 🧠 Объем оперативной памяти
- 💾 Использование дискового пространства
- ⏱️ Время работы системы (uptime)
- 🐚 Текущий shell и пользователь
- 🕐 Текущие дату и время
- 🌐 **Двуязычная поддержка** - английский и русский языки

## 🚀 Быстрый старт

### Вариант 1: Установка из .deb пакета (рекомендуется)

```bash
sudo dpkg -i myapp_1.0.0_all.deb
```

### Вариант 2: Сборка и установка с помощью скрипта

```bash
chmod +x build-and-install.sh
./build-and-install.sh
```

### Вариант 3: Установка из исходников

```bash
cd myapp
sudo python3 setup.py install
```

### Вариант 4: Установка с использованием pip

```bash
cd myapp
pip install -e .
```

## 📖 Использование

```bash
# Показать информацию на языке системы (или английском по умолчанию)
myapp

# Показать информацию на русском
myapp ru

# Показать информацию на английском
myapp en

# Показать справку
myapp --help
```

## 📤 Пример вывода

```
    ╔═══════════════════╗
    ║    MyApp Info     ║
    ╚═══════════════════╝

Пользователь........ user@ubuntu
ОС.................. Ubuntu 24.04.3 LTS
Ядро................ 6.8.0-1012-generic
Процессор........... Intel(R) Core(TM) i7-9700K (8 ядер)
Память.............. 16Gi
Диск................ 50G / 100G
Uptime.............. 5d 3h 42m
Shell............... bash
Время............... 2025-12-07 14:23:15
```

## 📁 Структура проекта

```
myapp/
├── myapp/                      # Пакет Python
│   ├── __init__.py             # Инициализация пакета
│   └── main.py                 # Основной модуль с классом SystemInfo
├── debian/                     # Файлы для упаковки в .deb
│   ├── control                 # Метаинформация пакета
│   ├── rules                   # Правила сборки
│   ├── changelog               # История изменений
│   ├── copyright               # Информация о лицензии
│   ├── compat                  # Версия debhelper
│   └── source/format           # Формат исходников
├── setup.py                    # Конфиг setup tools
├── README.md                   # Этот файл
└── build-and-install.sh        # Скрипт установки
```

## 🔧 Требования

- Python 3.6+
- Linux (Ubuntu, Debian, Fedora и т.д.)
- Доступ к файлам `/etc/os-release`, `/proc/cpuinfo`, `/proc/uptime`

## 📦 Удаление

```bash
sudo apt remove myapp
# или
sudo dpkg -r myapp
```

## 📝 Лицензия

MIT License - см. `debian/copyright` для подробностей.

## 👥 Автор

MyApp Team <team@myapp.dev>

## 🤝 Вклад

Всегда приветствуются pull requests!

## 👥 Автор

MyApp Team ylolvideo@gmail.com

## 🐛 Сообщение о проблемах

Если вы нашли ошибку, пожалуйста, откройте issue в репозитории.

## 🤝 Вклад

Всегда приветствуются pull requests!
