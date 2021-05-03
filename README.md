# discordbot

@client.command()
async def lick(ctx, member:str):
    lick = ['https://images-ext-2.discordapp.net/external/6qj8ymtgRYEdIyZ-m-3ep_8NywqpjB93Mv9ROPmnbeo/https/i.pinimg.com/originals/16/23/00/162300857841c32bd046374839b5d93f.gif']
    embed = discord.Embed(description=f"{ctx.author.mention} hat an {member} geleckt. <a:pepelove:822996861610360882>", color=0xFF0000)
    embed.set_image(url=f"{random.choice(lick)}")
    embed.set_footer(text=f"Angefordert von: {ctx.author}", icon_url=f"{ctx.author.avatar_url}")
    await ctx.send(embed=embed)
