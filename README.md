## Telegram чат-бот Gemini от Google.

https://t.me/GoogleZiBot

Диалог не запоминает.  
Работает в качестве справочника ответ-запрос.  
Парсит бесплатные прокси с сайта https://www.sslproxies.org/,  
что позволяет ему работать в странах, где Gemini не отвечает.  
Список прокси подгружает в Redis.  

### Команды бота:  
/start - старт бота  
/getproxy - обновить прокси  
/redis - список прокси в редисе (живут 10 минут - параметр LIFETIME)  
/country - адрес и страна последнего рабочего прокси  

### Параметры:  
PROXY = использовать прокси True | False  
TOKEN = токен Telegram бота  
API_KEY = Gemini API key  
MAX = колиство прокси из списка с сайта https://www.sslproxies.org/  
TIMEOUT = время ожидания ответа через каждый прокси в секундах  
LIFETIME = время жизни списка прокси в Redis (потом список обновляется)  
LOGLEVEL = уровень логирования  
