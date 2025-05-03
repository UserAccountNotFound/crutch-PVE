# crutch-PVE
костыли и лентяйки для ProxMox

## disable-PVE-Subscription
(Тестировалось на версии: 8x - 8.4.1)
Cкрипт вносит изменения в веб-интерфейс Proxmox Virtual Environment (PVE), отключащие уведомление (всплывающее окно) отсутствия платной подписки.

При выполнении скрипт ожидает один из двух параметров:

| **Option**       | **Description**                                                    |
|------------------|--------------------------------------------------------------------|
| `install`        | Установка изменений отключающих уведомление.                       |
| `uninstall`      | откат внесенных изменений (востановление из резервных копий).      |

### Install
Установливать под с правами привелегированной учетной записи (ака 'ROOT').
```
wget https://raw.githubusercontent.com/UserAccountNotFound/crutch-PVE/refs/heads/dev/disable-PVE-Subscription.sh
bash disable-PVE-Subscription.sh install
```
