# Zed Configurations

Мои персональные конфигурации для редактора [Zed](https://zed.dev/).

## 📦 Состав репозитория

- `settings.json` — основные настройки редактора (тема, шрифты, отступы, языковые серверы).
- `keymap.json` — пользовательские горячие клавиши и привязки.

## 🚀 Установка

### 1. Склонируйте и установите файлы конфигурации

**Для linux**:

```bash
# Пример для Linux (предварительно создайте резервную копию старых файлов!)
git clone https://github.com/a-kalki/zed-configs.git /tmp/zed-configs
cp /tmp/zed-configs/settings.json ~/.config/zed/settings.json
cp /tmp/zed-configs/keymap.json ~/.config/zed/keymap.json
```

**Для Windows (PowerShell)**:

```powershell
# 1. Перейдите в папку, где хотите хранить конфиги (например, Документы)
cd ~\Documents

# 2. Клонируйте репозиторий с GitHub
git clone https://github.com/a-kalki/zed-configs.git

# 3. Создайте папку конфигурации Zed (если её нет)
New-Item -ItemType Directory -Force -Path "$env:APPDATA\Zed"

# 4. Скопируйте файлы из клонированного репозитория в папку Zed
Copy-Item ".\zed-configs\settings.json" "$env:APPDATA\Zed\settings.json" -Force
Copy-Item ".\zed-configs\keymap.json" "$env:APPDATA\Zed\keymap.json" -Force
```

### 2. Перезапустите Zed

Перезапустите редактор, чтобы изменения вступили в силу.
