# Подробная инструкция по сборке и тестированию

Эта страница даёт более детальное руководство по подготовке окружения и базовому тестированию примеров.

## Установка на macOS

1. Установите Homebrew (если ещё не установлен):

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

2. Установите Python (рекомендуется через pyenv или brew) и создайте виртуальное окружение:

```bash
brew install pyenv  # опционально
python3 -m venv .venv
source .venv/bin/activate
```

3. Установите Panda3D:

```bash
pip install panda3d==1.10.13
```

## Установка на Windows

- Используйте официальный установщик Panda3D или pip в среде venv. Откройте PowerShell и выполните:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install panda3d==1.10.13
```

## Быстрая проверка примера

1. Активируйте виртуальное окружение.
2. Запустите `procedural-cube`:

```bash
python3 procedural-cube/main.py
```

Если окно Panda3D открылось и отобразился куб — окружение корректно настроено.
