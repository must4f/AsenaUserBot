<div align="center">
  <img src="https://i.imgyukle.com/2020/12/10/YcBPYR.jpg" width="200" height="200">
  <h1>Asena UserBot | forked version</h1>
</div>
<p align="center">
    Asena UserBot, Telegram kullanmanızı kolaylaştıran bir bottur. Tamamen açık kaynaklı ve ücretsizdir.
    <br>
        <a href="https://github.com/quiec/AsenaUserBot/blob/master/README.md#kurulum">Kurulum</a> |
        <a href="https://github.com/Quiec/AsenaUserBot/wiki/G%C3%BCncelleme">Güncelleme</a> |
        <a href="https://t.me/AsenaUserBot">Telegram Kanalı</a>
    <br>
</p>

----
![Docker Pulls](https://img.shields.io/docker/pulls/fusuf/asenauserbot?style=flat-square) ![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/fusuf/asenauserbot?style=flat-square)
## Kurulum
### Çok Basit Yöntem
yoq


### Basit Yöntem
Kurmak için tıklayın:

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/must4f/AsenaUserBot)
### Zor Yöntem
```python
git clone https://github.com/must4f/AsenaUserBot.git
cd AsenaUserBot
pip install -r requirements.txt
# Config.env oluşturun ve düzenleyin. #
python3 main.py
```

## Örnek Plugin
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
Help.add_info('@Fusuf tarafından yapılmıştır.') # Bilgi ekleyebilirsiniz.
# Ya da uyarı --> Help.add_warning('KULLANMA!')
Help.add() # Ve Ekleyelim.
```

## Bilgilendirme
Herhangi bir istek & şikâyet & öneri varsa [destek grubuna](https://t.me/AsenaSupport) ulaşabilirsiniz.

```
    Userbottan dolayı; Telegram hesabınız yasaklanabilir.
    Bu bir açık kaynaklı projedir, yaptığınız her işlemden kendiniz sorumlusunuz. Kesinlikle Asena yöneticileri sorumluluk kabul etmemektedir.
    Asenayı kurarak bu sorumlulukları kabul etmiş sayılırsınız.
```

## Credit
Thanks for;

[Seden UserBot](https://github.com/TeamDerUntergang/Telegram-UserBot)

[Userge](https://github.com/UsergeTeam/Userge)

[Spechide](https://github.com/Spechide)
