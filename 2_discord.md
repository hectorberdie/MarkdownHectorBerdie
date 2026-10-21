# Documentació del Bot de Discord
![Logotip de Discord](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQLueMtGyjZ7JkFpxIIaAjMJDhvz3tuSf_6TJg9o6jFTxC7CTu-stQv_ME&s=10)  

Pots registrar la teva aplicació al [Portal de Desenvolupadors de Discord.](https://discord.com/developers/applications)
Per fer que el bot respongui, escoltem l'esdeveniment `messageCreate` i utilitzem el mètode `message.reply()`.

``` JavaScript
client.on('messageCreate', message => {
  if (message.content === 'ping') {
    message.reply('pong!');
  }
});
```