Мы запускаем наш собственный проект Zapret VPN (под управлением Windows). 

## 1. Что это такое?
Данная программа имеет ряд преимуществ:
- Быстрые VPN сервера у крупного европейского провайдера
- Условно-бесплатное пользование (Вы можете доплачивать за доп. функции, но они не являются обязательными)
- Тонкость настройки (VPN работает как SOCKS прокси, следовательно позволяет тонко настраивать приложения, с которыми работает)

Пока происходит бета тест - все функции предоставляются бесплатно!

## 2. Установка программы
### 2.1. Скачайте и запустите RoskomFree
Скачать по ссылке: [пока недоступно]
<br>
Для запуска окна консоли и отладки запустите - `start.bat`
<br>
Для запуска в фоне запустите - `пока недоступно`

### 2.2. Установите расширение ZeroProxy
- Для Chrome https://chromewebstore.google.com/detail/proxy-switchyomega-3-zero/pfnededegaaopdmhkdmcofjmoldfiped
- Для Firefox https://addons.mozilla.org/en-US/firefox/addon/zeroomega/

### 2.3. Настройте расширение
Откройте настройки:

![image](https://github.com/user-attachments/assets/130ae337-7c04-4dc0-a154-7011a414e77d)

Введите заданный прокси (`127.0.0.1` и порт `18080`) (_тип оставьте `HTTP`_):

![image](https://github.com/user-attachments/assets/82e98b91-2f7a-4ce8-9db0-44f6ccef9a50)

Перейдите во вкладку `auto switch`:

![image](https://github.com/user-attachments/assets/4c65a761-0c8e-422a-91b7-5d5192d21fca)

Нажмите `Edit source code`

![image](https://github.com/user-attachments/assets/f0559845-4d10-45c2-941a-33ad8d93f4ce)

```python
[SwitchyOmega Conditions]
@with result

*.instagram.com +proxy
scontent-hel3-1.cdninstagram.com +proxy
*.cdninstagram.com +proxy
*.ntc.party +proxy
*.youtube.com +proxy
*.googlevideo.com +proxy
play.google.com +proxy
yt3.ggpht.com +proxy
youtu.be +proxy
*.discord.com +proxy
*.discord.gg +proxy
*.discordapp.com +proxy
*.discordapp.net +proxy
*.discord.media +proxy
*.discord-attachments-uploads-prd.storage.googleapis.com +proxy
*.dis.gd +proxy
*.discord.co +proxy
*.discordcdn.com +proxy
*.discordstatus.com +proxy
bbc.com +proxy
*.proton.me +proxy
twitter.com +proxy
*.twimg.com +proxy
t.co +proxy
x.com +proxy
*.torproject.org +proxy
*.rutracker.org +proxy 
*.rutracker.cc +proxy
*.archive.org +proxy
*.web.archive.org +proxy
*.soundcloud.com +proxy
*.mullvad.net +proxy
*.nnmclub.to +proxy
*.roskomsvoboda.org +proxy
holod.media +proxy
news.google.com +proxy
*.medium.com +proxy
*.habr.com +proxy
*.hybrid-analysis.com +proxy
*.4pda.to +proxy
*.chatgpt.com +proxy

* +direct
```

Сохраните изменения:

![image](https://github.com/user-attachments/assets/516ff29b-842c-4ebc-8403-12a83ce7d7ab)

Выйдите из настроек. Теперь Вам следует выбрать режим `auto switch`, нажав по иконке расширения (после успешного выбора он загорится синим):
