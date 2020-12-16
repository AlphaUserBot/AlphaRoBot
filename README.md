<div align="center">
  <img src="" width="200" height="200">
  <h1>Alpha UserBot</h1>
</div>
<p align="center">
    Alpha UserBot, Telegramdan istifadəni asanlaşdıran bir botdur.  Tamamilə açıq mənbəlidir və pulsuzdur.
    <br>
        <a href="https://github.com/FaridDadashzade/AlphaUserBot/blob/master/README.md#kurulum">Qurulum</a> |
        <a href="https://github.com/FaridDadashzade/AlphaUserBot/wiki/G%C3%BCncelleme">Güncəlləmə</a> |
        <a href="https://t.me/AlphaUserBot">Telegram Kanalı</a>
    <br>
</p>

----
![Docker Pulls](https://img.shields.io/docker/pulls/fusuf/asenauserbot?style=flat-square) ![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/fusuf/asenauserbot?style=flat-square)
## Qurulum
### Asan yol
[Youtube Videosu](https://www.youtube.com/watch?v=mUUQ53TYqI0) ![YouTube Video Views](https://img.shields.io/youtube/views/mUUQ53TYqI0?style=flat-square)

**Android:** Termuxu açın ve bu kodu yapıştırın: `bash <(curl -L https://kutt.it/88I5KA)`

**iOS:** iSH açın ve bu kodu yapıştırın: `apk update && apk add bash && apk add curl && curl -L -o asena_installer.sh https://t.ly/vATX && chmod +x asena_installer.sh && bash asena_installer.sh`

**Windows 10:** [Python](https://www.microsoft.com/en-us/p/python-38/9mssztt1n39l#activetab=pivot:overviewtab) indirin ardından PowerShell bu kodu yapıştırın: `Invoke-Expression (New-Object System.Net.WebClient).DownloadString('https://kutt.it/aYTzCx')`

### Basit Yöntem
Eğer botu kurma hakkında fikriniz yoksa burayı okuyunuz: [Kurulum Rehberi](https://github.com/Quiec/AsenaUserBot/wiki/Kurulum/)

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/FaridDadashzade/AlphaUserBot)
### Zor Yöntem
```python
git clone https://github.com/Quiec/AsenaUserBot.git
cd AsenaUserBot
pip install -r requirements.txt
# Config.env oluşturun ve düzenleyin. #
python3 main.py
```

## Plugin hazırlanması.
```python
from userbot.events import register
from userbot.cmdhelp import CmdHelp # <-- Bunu ekleyin.

@register(outgoing=True, pattern="^.deneme")
async def deneme(event):
    await event.edit('Gerçekten deneme!')

Help = CmdHelp('deneme') # Bilgi ekleyeceğiz diyoruz.
Help.add_command('deneme', # Komut
    None, # Komut parametresi varsa yazın yoksa None yazın
    'Gerçekten deneme yapıyor!', # Komut açıklaması
    'deneme' # Örnek kullanım.
    )
Help.add_info('@FaridDadashzade tərəfindən yaradılmışdır.) # Bilgi ekleyebilirsiniz.
# Ya da uyarı --> Help.add_warning('KULLANMA!')
Help.add() # Ve Ekleyelim.
```

## Support
Hərhansı bir problemlə qarşılaşdıqda [Dəstək Qrupumuza](https://t.me/AlphaDestek) yaza bilərsiniz.

```
    Userbot sayəsində;  Telegram hesabınız qadağan edilə bilər.
     Bu, açıq mənbəli bir layihədir, etdiyiniz hər şey üçün cavabdehsiniz.  Şübhəsiz ki, Asena rəhbərləri məsuliyyəti qəbul etmirlər.
     Alpha'nı quraraq, bu məsuliyyətləri qəbul etmiş sayılırsınız.
```

## Credit
Thanks for;

[Asena UserBot](https://github.com/Quiec/AsenaUserBot)

