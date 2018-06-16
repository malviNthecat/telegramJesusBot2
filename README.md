# telegramJesusBot2
Code for the bot

	 import telegramjesusbot

	TOKEN = "619398055:AAGrNsWoYaV1pCCAblWyETVm-_gPoe7jRzc"
	bot = telegramjesusbot.TeleBot(TOKEN)

	@bot.message_handler(commands=['start'])
	def start(m):
		msg = bot.send_message(m.chat.id, 'Привет, странник. Я все думал, когда же ты появишься')


def start(m):
	keyboard = types.ReplyKeyboardMarkup(resize_keyboard=True)
	keyboard.add(*[types.KeyboardButton(name) for name in ['Исповедь', 'Благословение', 'Контакты', 'Восхвалить Бога', 'Нажимать при плохом настроении']])

if m.text == 'Исповедь':
	bot.send_message(m.chat.id, 'Покайся в своих грехах', parse_mode='Markdown')
	keyboard = types.ReplyKeyboardMarkup(resize_keyboard=True)
	keyboard.add(*[types.KeyboardButton(name) for name in ['Пропустил дэдлайн', 'Комиссия впереди', 'Нет накопа', '...']])
elif m.text == 'Благословение':
	bot.send_message(m.chat.id, 'Бог в помощь', parse_mode='Markdown')
elif m.text == 'Контакты':
	bot.send_message(m.chat.id, 'Таир Алескеров - vk.com/tairufff , Третьяков Максим - vk.com/maximtretyakovru, Егор Шишкин - vk.com/shishkin_eg19', parse_mode ='Markdown')
elif m.text == 'Восхвалить бога':
	bot.send_message(m.chat.id, 'Номер карты (Сбербанк): 5469 3800 7648 6553', parse_mode='Markdown')
elif m.text == 'Нажимать про плохом настроении':
{
	bot.send_message(m.chat.id, 'Плохое настроение? Мы поможем! Выбери чем себя порадовать!')
