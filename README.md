# report_telegram_channels
Easily report multiple telegram channels
Легко оскаржуйте декілька телеграм каналів одночасно

## ENG
Attention: use on your own risk - telegram might ban your account if you will use this app to report huge amount of accounts in short time.
It's better to use separate telegram account to use this app.

Follow instructions [here](https://core.telegram.org/api/obtaining_api_id) 
to obtain your `api_id` and `api_hash` for telegram client

### Command Line
A script to easily report multiple telegram channels at once. Instruction:

1. Install python3 on your PC (if you do this on Windows, check Add To PATH on installation)
2. Open cmd/terminal and install telethon (`pip3 install telethon`) telegram client
3. Once you get your `api_id` and `api_hash`, run the python file attached to this message like this:
```shell
python3 report.py <api_id> <api_hash> "<report_message>" @channel1 @channel2 @channel3
```

### Docker

1. Install [Docker](https://www.docker.com/)
2. Build image: 
    ```shell
    docker build . -t report-telegram
    ```
3. Run:
    ```shell
    docker run -it --rm report-telegram <api_id> <api_hash> "<report_message>" @channel1 @channel2 @channel3
    ```

## UKR:

Увага: використовуйте на свій страх і ризик - телеграм може заблокувати ваш аккаунт якщо ви будете повідовляти про велику кількість аккаунтів за малий час.
Краще зробити окремий інстаграм акканунт для використання цієї програми.

Слідуйте інструкціям [тут](https://core.telegram.org/api/obtaining_api_id)
для того щоб отримати `api_id` та `api_hash` для telegram клієнту

### Інтерфейс командного рядка:
Python скрипт для оскаржування декількох телеграм каналів одночасно.

1. Встановіть python3 на вашому комп'ютері (якщо ви на Windows, відмітьте Add To PATH при інсталяції)
2. Відкрийте командний рядок(cmd)/термінал і встановіть telethon (`pip3 install telethon`) telegram клієнт
3. Коли ви отримаєте свій `api_id` та `api_hash`, запустіть python скрипт з цього репозиторію (скачайте і запустіть з командного рядка):
```shell
python3 report.py <api_id> <api_hash> "<зміст_повідомлення>" @channel1 @channel2 @channel3
```

### Docker

1. Встановіть [Docker](https://www.docker.com/)
2. Білд докер образу:
    ```shell
    docker build . -t report-telegram
    ```
3. Запуск:
    ```shell
    docker run -it --rm report-telegram <api_id> <api_hash> "<зміст_повідомлення>" @channel1 @channel2 @channel3
    ```
