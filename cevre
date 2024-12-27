import discord
from discord.ext import commands
import random

intents = discord.Intents.default()
intents.message_content = True

activities = [
    "Geri dönüştürülebilir atıkları geri dönüşüm kutusuna atın.",
    "Yanınızda tekrar kullanılabilir bir su şişesi taşıyın.",
    "Bugün araba yerine toplu taşıma veya bisiklet kullanın.",
    "Plastik poşet yerine bez çanta kullanın.",
    "Kullanmadığınız elektronik cihazların fişini çekin.",
    "Bugün suyu tasarruflu kullanmaya dikkat edin.",
    "Evde ışıkları gereksiz yere yakmamaya özen gösterin.",
    "Çevre dostu bir alışveriş listesi hazırlayın.",
    "Bütün yemeklerinizi bitirin, israf yapmamaya dikkat edin.",
    "Doğal malzemelerden yapılmış temizlik ürünleri kullanın.",
    "Plastik yerine cam veya metal kaplar kullanın.",
    "Evinizdeki eski kıyafetleri bağışlayın veya geri dönüştürün.",
    "Kendi bahçenizde organik sebzeler yetiştirmeye başlayın.",
    "Hızlı moda yerine sürdürülebilir markalardan alışveriş yapın.",
    "Yürüyüş yaparak doğayla iç içe vakit geçirin.",
    "Evdeki elektronik cihazları uzun süre kullanmadığınızda kapalı tutun.",
    "Geri dönüşüm yaparken, ambalajları doğru şekilde ayırdığınızdan emin olun.",
    "Plastik atık üretmeyi azaltarak, daha az paketli ürünler tercih edin.",
    "Her gün bir ağaç dikmeye çalışın veya doğaya faydalı bir şey yapın."
]

bot = commands.Bot(command_prefix='/')

@bot.event
async def on_ready():
    print(f"{bot.user} giriş yaptı!")

@bot.command()
async def start(ctx):
    await ctx.send("Merhaba! Çevre dostu öneriler almak için /aktivite yazabilirsiniz.")

@bot.command()
async def aktivite(ctx):
    activity = random.choice(activities)
    await ctx.send(f"Bugün yapabileceğiniz çevre dostu bir öneri: {activity}")

bot.run("")
