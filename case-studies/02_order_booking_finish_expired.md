Кейс 2
Партнёр пытается завершить процесс бронирования, обращается к методу Order Booking Finish, но создать заказ не выходит:  
```
Data in:
{
  "arrival_datetime": null,
  "book_timeout": null,
  "is_vip": null,
  "language": "en",
  "partner": {
    "amount_sell_b2b2c": "0",
    "comment": null,
    "partner_order_id": "100211111111111"
  },
  "payment_type": {
    "amount": "44",
    "currency_code": "USD",
    "init_uuid": null,
    "pay_uuid": null,
    "type": "deposit"
  },
  "return_path": null,
  "rooms": [
    {
      "guests": [
        {
          "age": null,
          "first_name": "han",
          "gender": null,
          "is_child": null,
          "last_name": "cai"
        }
      ]
    }
  ],
  "supplier_data": {
    "email": "In@ly.com",
    "first_name_original": "han",
    "last_name_original": "cai",
    "phone": "0123-4567890"
  },
  "upsell_data": null,
  "user": {
    "comment": null,
    "email": "In@ly.com",
    "phone": "0123-4567890"
  }
} 

Data out:
{
  "data": null,
  "debug": null,
  "error": "booking_form_expired",
  "status": "error"
}
```
В чём причина? 

  ---

  ### Мой ответ
  Из документации
Use partner_order_id field ending with booking_form_expired text on Booking Form stage
