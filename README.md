# board-with-mongo

 склонируйте этот репозитоиий
 перейдите  в папку с кодом 
 с помощью команды ` docker-compose up -d` запустите приложение. 

Если все успешно,запустятся три контейнера. 
Бекенд приложения стартует на 5000 порту. Чтобы воспользоваться приложением, нужно отправить запросы на адрес localhost:5000. В данном приложении доступны следующие эндпоинты: 
- POST message?text=text для создания нового сообщения с текстом text
- POST /tag/<message_id> добавление тега к существующему сообщению с id message_id. У тега есть обязательный аргумент text
- POST /comment/<message_id> добавление комментария к существующему сообщению с id message_id. У комментария есть обязательный аргумент text
- GET /message/message_id получение полного сообщения с тегами и комментариями по id
- GET /stats/message_id получение статистики по сообщению (количество тегов и комментариев) id
