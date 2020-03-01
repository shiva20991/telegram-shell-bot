# [Telegram Shell Bot]

This is a [Telegram](http://telegram.org) Bot to run shell commands. 

## Requirments

- Python 3.6+
- Pipenv

## Install
1. Create a bot and get token from [BotFather bot](https://telegram.me/BotFather)
1. Clone `Telegram Shell Bot`

        git clone https://github.com/vicalloy/telegram-shell-bot.git
        
1. Copy `settings.py.sample` to `settings.py` and config it.
    - `TOKEN` Bot token generated by BotFather
    - `ENABLED_USERS` Your telegram user id. Only enabled users can use this bot.  
    
1. Create a virtual environment and install required packages
        
        pipenv --python 3
        pipenv install -d --skip-lock
        pipenv shell

## Run

```
pipenv shell
python bot.py
```

## Usage

1. Take to bot, every input will tread as a shell commend.
1. `/pwd` show current working directory
1. `/ls` list directory contents
1. `/tasks` show all running tasks
1. `/kill` kill running task
1. `/sudo_login` call sudo
1. `/script` run scripts in ./scripts directory
