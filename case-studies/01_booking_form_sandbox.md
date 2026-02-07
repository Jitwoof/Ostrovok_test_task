## Кейс 1
_"Партнёр хочет начать процесс бронирование, вызывает метод Booking Form, но создать заказ не удаётся:_   
```
Data in:  
{  
  "book_hash": "h-c8833e24-1d3c-56ba-85a4-ca873e31f6fe",  
  "language": "ru",  
  "partner_order_id": "446245587863",  
  "user_ip": "00.111.0.1"  
}  
Data out:  
{  
  "data": null,  
  "debug": null,  
  "error": "sandbox_restriction",  
  "status": "error"  
}
```

Что ответим партнёру? 

---

### Мой ответ

По документации видно, что ошибка sandbox_restriction возникает, когда не настроен API-ключ. В Data-in не видно, чтобы какой-либо API-ключ вводился.  
Ответим, чтобы он API-ключ свой ввёл.  
