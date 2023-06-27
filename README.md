# Тестове завдання на позицію Backend розробника

## Технічні вимоги
- Використовувати лише стандартні компоненти Laravel 10
- Покриття тестами

## Функціональні вимоги

- Тестове завдання повинно працювати використовуючи наданий docker-compose (додайте необхідні контейнери)
- Написати класс клієнт для зовнішнього АРІ ([Документація з АРІ](api.MD))
- Написати команду яка буде парсити данні за допомогою створеного клієнту і зберігати їх в базу даних (створіть необхідну структуру БД)
- Написати метод який буде віддавати про компаніі. Вимоги до ендпоінту:
  - пагінація
  - можливість пошуку за назвою компанії/адресою або її частиною

Приклад відповіді
```json
{
  "data":[
    {
      "id":"1ee15eed-6baa-4732-afc0-f12c35b7dc25",
      "name":"Mixtape Inc.",
      "address":"1693 Alice Court, Annapolis MD 21401",
      "users":[
        {
          "id":"5a963e9b-ac97-4bd3-94af-64513f4ee3a0",
          "name_last":"Axelroad",
          "name_first":"Robert",
          "email":"b.axelroad@example.com",
          "position":"CEO"
        },
        ...
      ]
    },
    ...
  ]
}
```


