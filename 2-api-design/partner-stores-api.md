# Задание 2: проектирование API

## Запрос

```http
GET /api/v1/partner-stores?city=moscow
Host: api.petrushka-green.ru
Authorization: Bearer <token>
Accept: application/json
```

## Ответ
```json
{
  "ok": "true",
  "data": [
    {
      "id": "1",
      "name": "METRO",
      "logo_url": "https://cdn.petrushka-green.ru/logos/metro.png",
      "shop_url": "https://online.metro-cc.ru",
      "delivery": {
        "type": "timeslot",
        "label": "Ближайшая доставка",
        "date": "сегодня",
        "time_from": "21:00",
        "time_to": "23:00"
      }
    },
    {
      "id": "2",
      "name": "Ашан",
      "logo_url": "https://cdn.petrushka-green.ru/logos/auchan.png",
      "shop_url": "https://www.auchan.ru",
      "delivery": {
        "type": "timeslot",
        "label": "Ближайшая доставка",
        "date": "сегодня",
        "time_from": "18:00",
        "time_to": "20:00"
      }
    },
    {
      "id": "3",
      "name": "ВкусВилл",
      "logo_url": "https://cdn.petrushka-green.ru/logos/vkusvill.png",
      "shop_url": "https://vkusvill.ru",
      "delivery": {
        "type": "express",
        "label": "Быстрая доставка",
        "time_from_minutes": 20,
        "time_to_minutes": 60
      }
    },
    {
      "id": "4",
      "name": "ВИКТОРИЯ",
      "logo_url": "https://cdn.petrushka-green.ru/logos/victoria.png",
      "shop_url": "https://victoria-group.ru",
      "delivery": {
        "type": "timeslot",
        "label": "Ближайшая доставка",
        "date": "сегодня",
        "time_from": "17:00",
        "time_to": "19:00"
      }
    }
  ]
}
```
