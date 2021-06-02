# Graylog

sudo docker build . --tag microsevice_v1

sudo docker run -p 8000:8000 -d --name micro_v1 microsevice_v1

Работу сервиса можно проверить из консоли:

curl -X GET "http://127.0.0.1:8000/api/v1/hello" -H "accept: application/json"
curl -X GET "http://127.0.0.1:8000/api/v1/hello?name=World%20" -H "accept: application/json"

Или можно зайти в браузер и выполнить данные запросы
http://localhost:8000/docs/
