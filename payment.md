# Оплата

**Цель:** оплатить заказ банковской картой онлайн

## Основной сценарий:

1. Пользователь нажимает “оплатить заказ”
2. Система предлагает ввести данные банковской карты
3. Пользователь заполняет форму
4. Система отправляет данные о карте и сумме в платежный шлюз
5. Платежный шлюз совершает операцию по снятию денег и возвращает пользователя обратно в систему
6. Система проверяет оплату через платежный шлюз и меняет статус заказа, показываю пользователю, что заказ оплачен
7. Система передает заказ в готовку и доставку

## Альтернативный сценарий

1. Пользователь выбирает сохраненные данные карты и совершает оплату

## Исключения:

1. При ошибке платежного шлюза система показывает пользователю понятную ошибку
2. Если у пользователя не хватило денег на балансе и шлюз вернул ошибку - показать пользователю ошибку, что на балансе не хватает средств
3. Если при проверке оплаты шлюз вернул ошибку, показать пользователю сообщение о необходимости связаться со службой поддержки по телефону [PZ-14](https://skillfactory-sa-ikalinichenko.atlassian.net/browse/PZ-14)
