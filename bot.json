
const { Bot } = require("grammy");

const token = process.env.BOT_TOKEN;

if (!token) {
  throw new Error("8950689146:AAFB91-Zxmtp8Oc-3zsFHNGfkCVNQojGEKI");
}

const bot = new Bot(token);

bot.command("start", async (ctx) => {
  await ctx.reply(
    "Привет! 👋 Я твой Telegram-бот!\n" +
    "Я работаю на JavaScript.\n" +
    "Напиши мне сообщение!"
  );
});

bot.command("help", async (ctx) => {
  await ctx.reply(
    "Доступные команды:\n" +
    "/start — запуск\n" +
    "/help — помощь"
  );
});

bot.on("message:text", async (ctx) => {
  await ctx.reply("Ты написал: " + ctx.message.text);
});

bot.catch((err) => {
  console.error("Ошибка:", err.message);
});

bot.start();
console.log("Бот запущен!");
