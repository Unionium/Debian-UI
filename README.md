# Debian UI

Debian UI - Лёгкий автоскрипт установки настроенного окружения на Openbox для Debian 13.

_Форк [fakename00121v/debian-xp](https://github.com/fakename00121v/debian-xp)_

## Что это

`install_gui.sh` — bash-скрипт, который на чистой установке Debian 13 (профиль standard, без графики) ставит минимальное окружение на Openbox с темой и иконками Windows XP, панелью tint2, pcmanfm, lightdm и набором базовых приложений.

Скрипт рассчитан на новичков: запустил, дождался, перезагрузился, получил рабочий стол.

## Требования

- Debian 13 (trixie), установка с профилем **standard** (без рабочего стола и дисплей-менеджера)
- Доступ в интернет
- Права sudo
- Домашний каталог у пользователя, от которого выполняется запуск

Запуск от обычного пользователя:

```bash
bash <(curl -fsSL https://raw.githubusercontent.com/Unionium/Debian-UI/main/install_gui.sh)
```

Запуск от root не предусмотрен: конфиги копируются в `$HOME` текущего пользователя.

## После установки

```bash
sudo reboot
```

На экране входа LightDM выберите сессию Openbox.

## Лицензия

GPL v3. См. файл `LICENSE`.
