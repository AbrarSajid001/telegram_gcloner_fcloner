# telegram gcloner fcloner | Edited/Modified by EduTechTainMent (ETTM)

A Telegram bot to save Google Drive resources manually. If you have a good idea, please PR.

Demo robot: http://t.me/ahzhebot

## Instructions

### Ready to work

1. Install [Python 3.7+ (recommended the latest version 3.8)](https://www.python.org/downloads/)
2. Download [gclone](https://github.com/donwa/gclone/releases) or [fclone(recommended)](https://github.com/mawaya/rclone/releases)
3. Familiarize yourself with gclone and obtain the json containing the identity information of Service Accounts, and confirm that you can use `gclone` or `fclone` for related operations
4. Apply for a [Telegram Bot](https://core.telegram.org/bots#6-botfather) and get **token**
5. Get your own Telegram ID, for example through [this bot](https://t.me/userinfobot)

### Installation

Download the Zip version or download via git clone
```
$ git clone https://github.com/Waga43/telegram_gcloner_fcloner
```
Install dependencies through requirements.txt
```
$ pip3 install -r requirements.txt
```
Copy `config.ini.example` and rename it to `config.ini`
Modify the corresponding content, including:

> path_to_gclone = path of gclone.exe (If Linux distributions are obtained through installation, leave it blank. If Win has been added to the path, leave it blank. fclone must be filled in)
>
> telegram_token = telegram robot token
>
> user_ids = your telegram id (separated by commas, the first ID is the administrator)
>
> gclone_para_override = leave it blank if you don't know what this is

If you are interested, you can adjust the permissions in `./utils/restricted.py`, the default is to only respond to users in `user_ids`

## Run

1. Run `telegram_gcloner.py`.
2. Upload the ZIP file containing SA to the robot, and fill in `/sa` in the message title.
   -Mobile phone users can upload the ZIP file first, and then reply to the message `/sa`.
3. Send `/folders` to the robot to set frequently used folders.
4. Send or forward the information with the Google Drive link to the robot and follow the prompts.

All Credits to Original Dev: [wrenfairbank](https://github.com/wrenfairbank/telegram_gcloner)

## License

This project is licensed under the MIT License-see the [LICENSE](LICENSE) file for details
