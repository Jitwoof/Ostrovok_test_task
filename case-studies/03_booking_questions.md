## Кейс 3
Партнёр просит ответить на вопросы по бронированию:
- Какой тип оплаты? (Варианты: оплата картой в момент бронирования, оплата с имеющегося депозита, оплата в отеле)
- Какая стоимость бронирования? Есть ли дополнительные взносы, помимо указанной стоимости? Если да, то на какую сумму и за что?
- До какой даты (с указанием точного времени) можно отменить бронирование бесплатно?

```
{ "book_hash": "h-b7a573f0-22e4-5b84-b027-b94a2ea4e90c", "match_hash": "m-4f753b8f-9b3e-5e33-9389-c9d8a87c789b", "daily_prices": [ "4664.74" ], "meal": "nomeal", "payment_options": { "payment_types": [ { "amount": "380.00", "show_amount": "4664.74", "currency_code": "HKD", "show_currency_code": "RUB", "by": null, "is_need_credit_card_data": false, "is_need_cvc": false, "type": "hotel", "vat_data": { "included": false, "applied": false, "amount": "0.00", "currency_code": "RUB", "value": "0.00" }, "tax_data": { "taxes": [ { "name": "city_tax", "included_by_supplier": false, "amount": "100.00", "currency_code": "RUB" }, { "name": "cleaning_fee", "included_by_supplier": false, "amount": "1000.00", "currency_code": "RUB" } ] }, "perks": {}, "commission_info": { "show": { "amount_gross": "5033.00", "amount_net": "4664.74", "amount_commission": "368.26" }, "charge": { "amount_gross": "410.00", "amount_net": "380.00", "amount_commission": "30.00" } }, "cancellation_penalties": { "policies": [ { "start_at": null, "end_at": "2023-11-30T12:00:00", "amount_charge": "0.00", "amount_show": "0.00", "commission_info": { "show": { "amount_gross": "0.00", "amount_net": "0.00", "amount_commission": "0.00" }, "charge": { "amount_gross": "0.00", "amount_net": "0.00", "amount_commission": "0.00" } } }, { "start_at": "2023-11-30T12:00:00", "end_at": null, "amount_charge": "380.00", "amount_show": "4664.74", "commission_info": { "show": { "amount_gross": "5033.00", "amount_net": "4664.74", "amount_commission": "368.26" }, "charge": { "amount_gross": "410.00", "amount_net": "380.00", "amount_commission": "30.00" } } } ], "free_cancellation_before": "2023-11-30T12:00:00" }, "recommended_price": null } ] }, "bar_rate_price_data": null, "rg_ext": { "class": 3, "quality": 2, "sex": 0, "bathroom": 2, "bedding": 4, "family": 0, "capacity": 2, "club": 0, "bedrooms": 0, "balcony": 0, "view": 5, "floor": 0 }, "room_name": "Двухместный номер Стандарт с видом на город (2 отдельные кровати) (тип кровати может измениться)", "serp_filters": [ "has_bathroom" ], "sell_price_limits": null, "allotment": 729, "amenities_data": [ "non-smoking", "not-guaranteed" ], "any_residency": true, "deposit": null, "no_show": { "amount": "4636.00", "currency_code": "RUB", "from_time": "12:00:00" }, "room_data_trans": { "main_room_type": "Двухместный номер Стандарт с видом на город", "main_name": "Двухместный номер Стандарт с видом на город", "bathroom": null, "bedding_type": "2 отдельные кровати", "misc_room_type": "тип кровати может измениться" } }
```

---

### Мой ответ

Представим, что я пишу письмо Партнёру:

---
_Тема: Ответы на ваши вопросы по бронированию h-b7a573f0..._

_Здравствуйте!_

_На основе данных вашего бронирования (book_hash: h-b7a573f0...) отвечаем на вопросы:_

_1.  **Тип оплаты:** Оплата в отеле (`"type": "hotel"`). Гость производит расчёт непосредственно на месте заселения._  
_2.  **Стоимость:** Полная стоимость номера: 4 664.74 RUB.  
Да, также есть дополнительные сборы и они оплачиваются отдельно:  
Городской сбор (`city_tax`): 100.00 RUB.  
Плата за уборку (`cleaning_fee`): 1 000.00 RUB.  
3.  **Бесплатная отмена:** Бронирование можно отменить бесплатно **до 30 ноября 2023 года, 12:00 (UTC)**._

_Данные актуальны на момент формирования этого бронирования._

_С уважением,
Команда поддержки Ostrovok._
