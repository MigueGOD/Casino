
# Casino
comando casino discord.js










/// casino /// 
client.on("message", async message => {
  if(message.content === (prefix + 'casino')){
    message.channel.send(`Espera...`).then((msg) => {
       let thumb = ["🍒 🍕 🍒", "💎 🍕 🍊", "🍒 🍇 💎", "🍊 🍓 🍊", "🍌 🍌 🍓", "🍎 🍊 🍎", "🍐 🍕 🍇", "🍒 🍊 🍌", "🍒 💎 💎 ", "🍌 :seven: 🍕", "🍒 🍒 🍒", "🍕 🍕 🍕", "🍓 🍓 🍓", "🍌 🍌 🍌", "🍇 🍇 🍇", "🍎 🍎 🍎", "💎 💎 💎", ":seven: :seven: :seven:"]

      

       var enlace = thumb[Math.floor(Math.random() * thumb.length)]

        
       const embed = new MessageEmbed()
       .setTitle("Casino Game")
       .setDescription(enlace)
         
         .setTimestamp()
         .setColor("RED")
         msg.edit(embed);
         msg.edit("\u200B");
    })
  }
});
