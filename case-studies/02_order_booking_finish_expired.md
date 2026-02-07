## Кейс 2  
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

Представим, что я пишу письмо Партнёру:

---

_Тема: Ошибка «booking_form_expired» при вызове Order Booking Finish_

_Здравствуйте!_

_Проанализировали ваш запрос на завершение бронирования. Ошибка «booking_form_expired» означает, что сессия бронирования истекла._

_В вашем запросе обнаружено поле `"partner_order_id": "100211111111111"`. Если этот ID был сформирован с использованием суффикса `_booking_form_expired`, наша система специально имитирует ситуацию истёкшей сессии — это стандартный способ тестирования такого сценария._

_**Решение:**_  
_1.  Проверьте логику формирования `partner_order_id` в вашей системе. Убедитесь, что для реальных броней не используется тестовый суффикс._  
_2.  Убедитесь, что между вызовом метода `Booking Form` и `Order Booking Finish` проходит не более **15-20 минут** (стандартный таймаут сессии)._

_Если вы не использовали тестовый суффикс, пришлите, пожалуйста, точное время обоих запросов — мы проверим логи на нашей стороне._

_С уважением,
Команда поддержки Ostrovok._
