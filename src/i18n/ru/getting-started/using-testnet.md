# Использование руководства по Testnet

Последнее обновление для testnet2

---

## Зачем использовать Testnet?

Testnet - отличное место, где Вы можете экспериментировать с приложениями Decred, не опасаясь, что ошибка будет стоить Вам реальных денег. На самом деле рекомендовано использовать testnet для изучения основ программного обеспечения Decred и любых новых характеристик.

Decred в настоящее время использует свой второй Testnet, также известный как testnet2. Тестовые сети периодически перезагружаются, чтобы сохранить удобные для оперирования размеры файлов блокчейна.

---

## Как запустить узел Testnet (Testnet Node)

Управлять узлом testnet2 чрезвычайно просто. Выбранному Вами приложению нужно будет загрузить блокчейн testnet2, и Вам надо будет создать новый файл кошелька для использования в testnet2. Ваш блокчейн основной сети и файлы кошельков останутся нетронутыми. Переключаться между ними чрезвычайно просто.

---

## Paymetheus

Чтобы запустить `Paymetheus` в testnet2, просто запустите приложение `Decred Testnet` вместо обычного приложения `Decred`. Затем Вас проведуть через создание кошелька (те же шаги в "Руководстве по настройке Paymetheus" [Paymetheus Setup guide](/getting-started/user-guides/paymetheus.md)). После того, как `dcrd` завершает синхронизацию в фоновом режиме, Вы сможете заполнить свой кошелек `Paymetheus` тестовыми DCR и ознакомиться с программным обеспечением.

---

## Decrediton 

Чтобы запустить `Decrediton` в testnet2, Вы должны запустить `Decrediton` из командной строки с флагом `--testnet`. Имейте в виду, что использование флага один раз приведет к тому, что программа всегда будет запускаться в этом режиме, пока Вы не используете флаг `--mainnet` , чтобы переключиться обратно на блокчейн основной сети.

Для Linux, 

1. Откройте terminal и перейдите в каталог с исполняемым файлом decrediton.
2. Выведите команду `./decrediton --testnet`.
3. Decrediton запустится и попытается подключиться к testnet2.

For macOS,

1. Откройте terminal и выполните следующую команду: `/Applications/decrediton.app/Contents/MacOS/decrediton --testnet`
2. Decrediton запустится и попытается подключиться к testnet2.

Помните, что если Вы захотите переключить Decrediton на основную сеть mainnet, Вам нужно будет задать эти команды с флагом `--mainnet`.

___ 

## Набор команд для командной строки

Чтобы запустить `dcrd` и `dcrwallet` в тестовой сети, просто добавьте флаг `--testnet` к Вашей команде запуска. В качестве альтернативы Вы можете прописать `testnet=1` во все Ваши конфигурационные файлы, но, как правило, гораздо быстрее использовать флаг запуска startup.

При первом запуске `dcrd --testnet`, `dcrd` начнет загружать блокчейн testnet2 в папку `data/testnet2` в домашнем каталоге `dcrd`.

Прежде чем Вы сможете запустить `dcrwallet` с флагом `--testnet`, Вы должны создать отдельный кошелек testnet, используя команду `dcrwallet --testnet --create`. Шаги те же, что и в [dcrwallet Setup Guide](/getting-started/user-guides/dcrwallet-setup.md). 

Чтобы задавать команды `dcrwallet` и `dcrd`, Вы также должны добавить флаг `--testnet` во все команды  `dcrctl`, которые Вы используете. Например, Вы должны задать команду `dcrctl --testnet --wallet getbalance`, чтобы проверить свой баланс testnet. 

---

## Приобретение монет Testnet

Вы можете приобрести монеты через [Decred Testnet Faucet](https://faucet.decred.org). Пожалуйста, верните все монеты по адресу, указанному внизу той страницы, когда Вы закончите практиковаться с testnet.

---

