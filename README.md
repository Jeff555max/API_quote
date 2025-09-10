Случайные цитаты из https://api.quotable.io/random

Random Quote Generator

Веб-приложение на Flask, которое показывает случайные цитаты из API Quotable. 

🚀 Возможности

📖 Случайные цитаты - Получение случайных цитат из публичного API

⚡ Быстрая работа - Мгновенная загрузка новых цитат

🔒 Безопасность - Настроенный секретный ключ для Flask-сессий

🛠️ Технологии
Backend: Python 3, Flask

Frontend: HTML, CSS 

API: Quotable.io

HTTP-клиент: Requests

📦 Установка и запуск
1. Клонирование репозитория

git clone https://github.com/ваш-username/random-quote-generator.git

cd random-quote-generator

2. Создание виртуального окружения


python -m venv venv
source venv/bin/activate  # Linux/MacOS

или

venv\Scripts\activate     # Windows

3. Установка зависимостей

pip install -r requirements.txt

4. Запуск приложения

python app.py

Приложение будет доступно по адресу: http://localhost:5000

🔧 Настройка
Конфигурационные параметры
python
app.config['SECRET_KEY'] = 'your_secret_key'  # Замените на надежный ключ

Важные заметки по безопасности
⚠️ Внимание: В текущей реализации отключена проверка SSL-сертификатов (verify=False). Для production-среды:

Установите сертификаты:

pip install certifi
Используйте безопасное подключение:

python
import certifi
response = requests.get('https://api.quotable.io/random', verify=certifi.where())

🌐 API Endpoints
GET / - Главная страница со случайной цитатой

🐛 Решение проблем
Ошибка SSL сертификата
Если возникает ошибка SSLCertVerificationError:

# Обновление сертификатов системы
sudo update-ca-certificates  # Linux

📄 Лицензия
Этот проект распространяется под лицензией MIT. 

👨‍💻 Автор
Разработано с ❤️ к Flask и веб-разработке
