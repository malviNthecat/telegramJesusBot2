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
	keyboard.add(*[types.KeyboardButton(name) for name in ['Исповедь', 'Благословение', 'Контакты', 'Восхвалить Бога', 'Нажимать при 	плохом настроении']])

	if m.text == 'Исповедь':
	bot.send_message(m.chat.id, 'Покайся в своих грехах', parse_mode='Markdown')
	keyboard = types.ReplyKeyboardMarkup(resize_keyboard=True)
	keyboard.add(*[types.KeyboardButton(name) for name in ['Пропустил дэдлайн', 'Комиссия впереди', 'Нет накопа', '...']])
	elif m.text == 'Благословение':
	bot.send_message(m.chat.id, 'Бог в помощь', parse_mode='Markdown')
	elif m.text == 'Контакты':
		bot.send_message(m.chat.id, 'Таир Алескеров - vk.com/tairufff , Третьяков Максим - vk.com/maximtretyakovru, Егор Шишкин 		- vk.com/shishkin_eg19', parse_mode ='Markdown')
	elif m.text == 'Восхвалить бога':
	bot.send_message(m.chat.id, 'Номер карты (Сбербанк): 5469 3800 7648 6553', parse_mode='Markdown')
	elif m.text == 'Нажимать про плохом настроении':
	{
	bot.send_message(m.chat.id, 'Плохое настроение? Мы поможем! Выбери чем себя порадовать!')
	keyboard = types.ReplyKeyboardMarkup(resize_keyboard=True)
	keyboard.add(*[types.KeyboardButton(name) for name in ['Фильмы', 'Мемы']])
		if m.text == 'Фильмы':
			bot.send_message(m.chat.id, 'Выбери жанр фильма', parse_mode='Markdown')
			keyboard = types.ReplyKeyboardMarkup(resize_keyboard=True)
			keyboard.add(*[types.KeyboardButton(name) for name in ['Боевики', 'Комедия', 'Комиксы', ''Мультфильмы]])
				if m.text == 'Комиксы':
					bot.send_message(m.chat.id, 'Топ-10 комиксов 1. Темный рыцарь (2008) kp 8.5 IMDb 9 2. Темный Рыцарь: Возрождение легенды (2012) kp 8.1 IMDb 8.4 3. Люди в черном (1997) kp 7.9 IMDb 7.3 4. Маска (1994) kp 7.9 IMDb 6.9 5. Олдбой (2003) kp 8.1 IMDb 8.4 6. Бэтмен: Начало (2005) kp 7.9 IMDb 8.3 7. Мстители (2012) kp 7.8 IMDb 8.1 8. Люди Икс: Дни минувшего будущего (2014) kp 7.7 IMDb 8 9. Город Грехов (2005) kp 7.8 IMDb 8 10. Стражи Галактики (2014) kp 7.7 IMDb 8.2', parse_mode='Markdown')
				elif m.text == 'Боевики':
					bot.send_message(m.chat.id, '1. Начало (2010) kp 8.6 IMDb 8.8 2. Гладиатор (2000) kp 8.5 IMDb 8.5 3. Матрица (1999) kp 8.4 IMDb 8.7 4. Большой Куш (2000) kp 8.5 IMDb 8.3 5. Пираты Карибского Моря: Проклятие Черной Жемчужины (2003) kp 8.3 IMDb 8 6. Терминатор 2: Судный день (1991) kp 8.3 IMDb 8.5 7. Назад в Будущее 2 (1989) kp 8.2 IMDb 7.8 8. Брат (1997) kp 8.2 IMDb 8 9. Мстители: Война Бесконечности (2018) kp 8 IMDb 8.8 10. Пятый Элемент (1997) kp 8 IMDb 7.7', parse_mode='Markdown')
				elif m.text == 'Комедия':
					bot.send_message(m.chat.id,'Комедии 1. 1+1 (2011) kp 8.8 IMDb 8.5 2. Иван Васильевич меняет професию (1973) kp 8.7 IMDb 8.4 3. Жизнь Прекрасна (1997) kp 8.6 IMDb 8.6 4. Достучаться до небес (1997) kp 8.6 IMDb 8 5. Криминальное чтиво (1994) kp 8.6 IMDb 8.9 6. Операция "Ы" и другие приключения Шурика (1965) kp 8.7 IMDb 8.6 7. Назад в будущее (1985) kp 8.6 IMDb 8.5 8. Карты, деньги, два ствола (1998) kp 8.5 IMDb 8.2 9. Бриллиантовая рука (1968) kp 8.5 IMDb 8.5 10. В бой идут одни старики (1973) kp 8.7 IMDb 8.5', parse_mode='Markdown')
				elif m.text == 'Мультфильмы':
					bot.send_message(m.chat.id,'1. Король Лев (1994) kp 8.7 IMDb 8.5 2. Тайна Коко (2017) kp 8.6 IMDb 8.5 3. ВАЛЛ И (2008) kp 8.3 IMDb 8.5 4. Как приручить дракона (2010) kp 8.2 IMDb 8.4 5. Зверополис (2016) kp 8.3 IMDb 8.3 6. Красавица и Чудовище (1991) kp 8.2 IMDb 8.2 7. Балто (1995) kp 8.2 IMDb 8 8. Остров собак (2018) kp 8.4 IMDb 8.2 9. Аладдин (1992) kp 8.1 IMDb 8 10. Головоломка (2015) kp 8 IMDb 8.2', parse_mode = 'Markdown')
	}

		bot.polling()
