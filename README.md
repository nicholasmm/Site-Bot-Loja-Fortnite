# Instruções para setar ambiente de desenvolvimento

### Requisitos básicos

1. Abra o telegram e procure por <span style="color:aqua;">@BotFather</span>.

2. Clique em <span style="color:aqua;">Start</span>.

3. Digite <span style="color:aqua;">/newbot</span>. e escolha um nome para o bot, além de um nome de usuário.

4. Copie o token gerado pelo BotFather e coloque em um arquivo **.env**, atribua o token há uma variável de nome *TOKEN* ou *BOT_TOKEN*. <span style="color:red">Não faça o upload do arquivo .env para o git</span>.

5. Instale a biblioteca *python-telegram-bot* com o comando: \
```pip install python-telegram-bot```

6. Agora é só escrever o script que manejará a API.

### Estrutura básica

```
import telegram
from telegram.ext import Updater, CommandHandler

updater = Updater(token='TOKEN', use_context=True)
```
