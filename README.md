# MyApp v1.0.0 - System Information Utility

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.6+](https://img.shields.io/badge/Python-3.6+-blue.svg)](https://www.python.org/downloads/)
[![Status: Active](https://img.shields.io/badge/Status-Active-green.svg)]()
[![Documentation](https://img.shields.io/badge/Docs-Complete-blue.svg)]()

**English** | [Русский](#-русский)

---

## 📋 English

**MyApp** is a command-line utility for displaying system information, similar to the popular **neofetch** program, but written in Python. It provides comprehensive system details in a beautiful formatted output.

### ✨ What's New in v1.0.0

- ✅ **Dependency Checking** - Automatic verification of all requirements before installation
- ✅ **Multi-OS Support** - Works on Linux (✅ full), macOS (🟡 in dev), Windows (🟡 WSL 2)
- ✅ **Smart Installer** - Automatic PATH management and dependency installation
- ✅ **Complete Documentation** - 12 comprehensive guides in 2 languages
- ✅ **Professional Quality** - Clean code with error handling and best practices

### 🌟 Core Features

- 📋 Display OS and Linux distribution information
- 🔧 Linux kernel version information  
- 💻 CPU details (model and number of cores)
- 🧠 RAM size
- 💾 Disk space usage
- ⏱️ System uptime
- 🐚 Current shell and user
- 🕐 Current date and time
- 🌐 **Bilingual support** - English and Russian
- 🎯 **Smart Installation** - Automatic dependency checking
- 🖥️ **Multi-OS Support** - Linux, macOS, Windows (WSL 2)
- 📚 **Complete Docs** - 12 guides on 2 languages

---

### 🚀 Quick Start (3 Steps)

#### Option 1: Smart Installer (Recommended) ⭐

```bash
# 1. Make installer executable
chmod +x install-myapp.sh

# 2. Run smart installer
./install-myapp.sh

# 3. Restart terminal and use
exit
myapp
```

**What it does automatically:**
- ✅ Checks Python version (3.6+)
- ✅ Checks pip and setuptools
- ✅ Installs missing packages
- ✅ Installs MyApp
- ✅ Adds to PATH
- ✅ Tests installation

#### Option 2: Ubuntu/Debian Package

```bash
sudo dpkg -i myapp_1.0.0_all.deb
myapp
```

#### Option 3: From Source

```bash
cd myapp
sudo python3 setup.py install
myapp
```

#### Option 4: Using pip

```bash
cd myapp
pip install -e .
myapp
```

---

### 📖 Usage

```bash
# Show system information
myapp

# Show in Russian
myapp ru

# Show in English
myapp en

# Show help
myapp --help
```

---

### 📤 Example Output

```
    ╔═══════════════════╗
    ║    MyApp Info     ║
    ╚═══════════════════╝

User..................... user@ubuntu
OS....................... Ubuntu 24.04.3 LTS
Kernel................... 6.8.0-1030-azure
CPU...................... Intel(R) Xeon(R) Platinum 8370C (2 cores)
RAM...................... 7.8Gi
Disk..................... 11G / 32G
Uptime................... 0d 0h 16m
Shell.................... bash
Time..................... 2025-12-07 21:39:28
```

---

### 📚 Documentation

Start with these guides:

| Document | Time | For Whom |
|----------|------|----------|
| **[DOCUMENTATION_INDEX.md](DOCUMENTATION_INDEX.md)** | 5 min | **START HERE** ⭐ |
| **[GETTING_STARTED.md](GETTING_STARTED.md)** | 5 min | Quick start |
| **[DOWNLOAD_AND_INSTALL.md](DOWNLOAD_AND_INSTALL.md)** | 10 min | Installation guide |
| **[METHODS_COMPARISON.md](METHODS_COMPARISON.md)** | 8 min | Choose method |
| [OS_SUPPORT.md](OS_SUPPORT.md) | 10 min | Different OS |
| [IMPROVEMENTS.md](IMPROVEMENTS.md) | 15 min | What's new |
| [QUICK_START.md](QUICK_START.md) | 3 min | Reference |
| [GITHUB_UPLOAD_GUIDE.md](GITHUB_UPLOAD_GUIDE.md) | 5 min | Upload to GitHub |

**Full documentation: ~85 KB, 3000+ lines, 100+ code examples**

---

### 🖥️ Supported Operating Systems

| OS | Status | Notes |
|----|--------|-------|
| **Linux** | ✅ Full | Ubuntu, Debian, Fedora, CentOS, Arch |
| **macOS** | 🟡 Dev | 10.14+, M1/M2/M3 compatible |
| **Windows** | 🟡 Dev | WSL 2 recommended |

---

### ✅ Dependency Checking

Before installation, check if all dependencies are available:

```bash
python3 -m myapp.dependencies
```

This checks:
- ✅ Python 3.6+
- ✅ pip
- ✅ setuptools
- ✅ OS compatibility

---

### 🔧 Project Structure

```
myapp/
├── myapp/                          # Python package
│   ├── __init__.py                 # Initialization
│   ├── main.py                     # Core application
│   ├── dependencies.py             # ✨ NEW: Dependency checker
│   └── path_manager.py             # ✨ NEW: PATH management
├── debian/                         # .deb packaging files
│   ├── control, rules, changelog
│   └── copyright, compat
├── setup.py                        # Package configuration
├── install-myapp.sh                # ✨ NEW: Smart installer
├── build-and-install.sh            # Alternative installer
├── README.md                       # This file
├── DOCUMENTATION_INDEX.md          # Docs index
├── GETTING_STARTED.md              # Quick start
├── DOWNLOAD_AND_INSTALL.md         # Installation guide
├── METHODS_COMPARISON.md           # Method comparison
├── OS_SUPPORT.md                   # OS-specific guides
├── IMPROVEMENTS.md                 # What's new
├── QUICK_START.md                  # Quick reference
├── GITHUB_UPLOAD_GUIDE.md          # GitHub upload
├── INSTALL.md                      # Install reference
├── PROJECT_SUMMARY.md              # Project overview
└── DOWNLOAD.md                     # Download info
```

---

### 🔧 Requirements

- **Python**: 3.6 or higher
- **OS**: Linux (Ubuntu, Debian, Fedora, CentOS, Arch, etc.)
- **Access**: `/etc/os-release`, `/proc/cpuinfo`, `/proc/uptime`

---

### 📦 Uninstall

```bash
# If installed from .deb
sudo apt remove myapp

# If installed from pip
pip uninstall myapp

# If installed from source
sudo pip uninstall myapp
```

---

### 🔄 Update

```bash
# From pip
pip install --upgrade myapp

# From source
cd myapp && git pull && pip install --upgrade -e .

# From .deb
sudo dpkg -i myapp_1.0.0_all.deb
```

---

### 🐛 Troubleshooting

**"myapp: command not found"**
```bash
# Reload terminal
source ~/.bashrc

# Or add to PATH
export PATH="$HOME/.local/bin:$PATH"
```

**"Python not found"**
```bash
# Linux
sudo apt-get install python3 python3-pip

# macOS
brew install python3
```

See [DOWNLOAD_AND_INSTALL.md](DOWNLOAD_AND_INSTALL.md) for complete troubleshooting.

---

### 📝 License

MIT License - see [debian/copyright](myapp/debian/copyright) for details.

### 👥 Author

MyApp Team <team@myapp.dev>

### 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

---

---

## 📋 Русский

**MyApp** - утилита командной строки для отображения информации о системе, аналогичная популярной программе **neofetch**, но написанная на Python. Она предоставляет полную информацию о системе в красиво отформатированном выводе.

### ✨ Новое в v1.0.0

- ✅ **Проверка зависимостей** - Автоматическая проверка всех требований перед установкой
- ✅ **Поддержка нескольких ОС** - Работает на Linux (✅ полная), macOS (🟡 разработка), Windows (🟡 WSL 2)
- ✅ **Умный установщик** - Автоматическое управление PATH и установка зависимостей
- ✅ **Полная документация** - 12 подробных руководств на 2 языках
- ✅ **Профессиональное качество** - Чистый код с обработкой ошибок

### 🌟 Основные возможности

- 📋 Отображение информации об ОС и дистрибутиве Linux
- 🔧 Информация о версии ядра
- 💻 Сведения о процессоре (модель и количество ядер)
- 🧠 Объем оперативной памяти
- 💾 Использование дискового пространства
- ⏱️ Время работы системы (uptime)
- 🐚 Текущий shell и пользователь
- 🕐 Текущие дату и время
- 🌐 **Двуязычная поддержка** - английский и русский
- 🎯 **Умная установка** - Автоматическая проверка зависимостей
- 🖥️ **Поддержка нескольких ОС** - Linux, macOS, Windows (WSL 2)
- 📚 **Полная документация** - 12 руководств на 2 языках

---

### 🚀 Быстрый старт (3 шага)

#### Вариант 1: Умный установщик (Рекомендуется) ⭐

```bash
# 1. Сделать установщик исполняемым
chmod +x install-myapp.sh

# 2. Запустить умный установщик
./install-myapp.sh

# 3. Перезагрузить терминал и использовать
exit
myapp
```

**Что он делает автоматически:**
- ✅ Проверяет версию Python (3.6+)
- ✅ Проверяет pip и setuptools
- ✅ Устанавливает недостающие пакеты
- ✅ Устанавливает MyApp
- ✅ Добавляет в PATH
- ✅ Проверяет установку

#### Вариант 2: Пакет Ubuntu/Debian

```bash
sudo dpkg -i myapp_1.0.0_all.deb
myapp
```

#### Вариант 3: Из исходников

```bash
cd myapp
sudo python3 setup.py install
myapp
```

#### Вариант 4: Используя pip

```bash
cd myapp
pip install -e .
myapp
```

---

### 📖 Использование

```bash
# Показать информацию о системе
myapp

# Показать на русском
myapp ru

# Показать на английском
myapp en

# Показать справку
myapp --help
```

---

### 📤 Пример вывода

```
    ╔═══════════════════╗
    ║      MyApp Info    ║
    ╚═══════════════════╝

Пользователь........ user@ubuntu
ОС.................. Ubuntu 24.04.3 LTS
Ядро................ 6.8.0-1030-azure
Процессор........... Intel(R) Xeon(R) Platinum 8370C (2 ядер)
Память.............. 7.8Gi
Диск................ 11G / 32G
Uptime.............. 0d 0h 16m
Shell............... bash
Время............... 2025-12-07 21:39:28
```

---

### 📚 Документация

Начните с этих руководств:

| Документ | Время | Для кого |
|----------|-------|----------|
| **[DOCUMENTATION_INDEX.md](DOCUMENTATION_INDEX.md)** | 5 мин | **НАЧНИТЕ ОТСЮДА** ⭐ |
| **[GETTING_STARTED.md](GETTING_STARTED.md)** | 5 мин | Быстрый старт |
| **[DOWNLOAD_AND_INSTALL.md](DOWNLOAD_AND_INSTALL.md)** | 10 мин | Руководство установки |
| **[METHODS_COMPARISON.md](METHODS_COMPARISON.md)** | 8 мин | Выбор метода |
| [OS_SUPPORT.md](OS_SUPPORT.md) | 10 мин | Для разных ОС |
| [IMPROVEMENTS.md](IMPROVEMENTS.md) | 15 мин | Что нового |
| [QUICK_START.md](QUICK_START.md) | 3 мин | Справка |
| [GITHUB_UPLOAD_GUIDE.md](GITHUB_UPLOAD_GUIDE.md) | 5 мин | Загрузка на GitHub |

**Полная документация: ~85 KB, 3000+ строк, 100+ примеров кода**

---

### 🖥️ Поддерживаемые операционные системы

| ОС | Статус | Примечания |
|----|--------|-----------|
| **Linux** | ✅ Полная | Ubuntu, Debian, Fedora, CentOS, Arch |
| **macOS** | 🟡 Разработка | 10.14+, совместима M1/M2/M3 |
| **Windows** | 🟡 Разработка | WSL 2 рекомендуется |

---

### ✅ Проверка зависимостей

Перед установкой проверьте наличие всех зависимостей:

```bash
python3 -m myapp.dependencies
```

Проверяет:
- ✅ Python 3.6+
- ✅ pip
- ✅ setuptools
- ✅ Совместимость ОС

---

### 🔧 Структура проекта

```
myapp/
├── myapp/                          # Пакет Python
│   ├── __init__.py                 # Инициализация
│   ├── main.py                     # Основное приложение
│   ├── dependencies.py             # ✨ НОВОЕ: Проверка зависимостей
│   └── path_manager.py             # ✨ НОВОЕ: Управление PATH
├── debian/                         # Файлы .deb упаковки
│   ├── control, rules, changelog
│   └── copyright, compat
├── setup.py                        # Конфиг пакета
├── install-myapp.sh                # ✨ НОВОЕ: Умный установщик
├── build-and-install.sh            # Альтернативный установщик
├── README.md                       # Этот файл
├── DOCUMENTATION_INDEX.md          # Индекс документации
├── GETTING_STARTED.md              # Быстрый старт
├── DOWNLOAD_AND_INSTALL.md         # Руководство установки
├── METHODS_COMPARISON.md           # Сравнение методов
├── OS_SUPPORT.md                   # Инструкции для разных ОС
├── IMPROVEMENTS.md                 # Что нового
├── QUICK_START.md                  # Быстрая справка
├── GITHUB_UPLOAD_GUIDE.md          # Загрузка на GitHub
├── INSTALL.md                      # Справочник установки
├── PROJECT_SUMMARY.md              # Обзор проекта
└── DOWNLOAD.md                     # Информация о скачивании
```

---

### 🔧 Требования

- **Python**: 3.6 или выше
- **ОС**: Linux (Ubuntu, Debian, Fedora, CentOS, Arch и т.д.)
- **Доступ**: `/etc/os-release`, `/proc/cpuinfo`, `/proc/uptime`

---

### 📦 Удаление

```bash
# Если установлено из .deb
sudo apt remove myapp

# Если установлено из pip
pip uninstall myapp

# Если установлено из исходников
sudo pip uninstall myapp
```

---

### 🔄 Обновление

```bash
# Из pip
pip install --upgrade myapp

# Из исходников
cd myapp && git pull && pip install --upgrade -e .

# Из .deb
sudo dpkg -i myapp_1.0.0_all.deb
```

---

### 🐛 Решение проблем

**"myapp: команда не найдена"**
```bash
# Перезагрузить терминал
source ~/.bashrc

# Или добавить в PATH
export PATH="$HOME/.local/bin:$PATH"
```

**"Python не найден"**
```bash
# Linux
sudo apt-get install python3 python3-pip

# macOS
brew install python3
```

Смотрите [DOWNLOAD_AND_INSTALL.md](DOWNLOAD_AND_INSTALL.md) для полного решения проблем.

---

### 📝 Лицензия

MIT License - см. [debian/copyright](myapp/debian/copyright) для подробностей.

### 👥 Автор

MyApp Team <team@myapp.dev>

### 🤝 Вклад

Вклад приветствуется! Пожалуйста, отправляйте Pull Requests.

---

**Версия**: 1.0.0  
**Дата**: 2025-12-07  
**Статус**: ✅ Активный  
**Лицензия**: MIT
