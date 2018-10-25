# Book-Shop_T6
Tasks from 6 lesson

1. В шаблоне компонента ProcessOrderFormComponent добавить поле дата доставки.
2. Реализовать ProcessOrderFormComponent в виде реактивной формы.
3. Добавить валидаторы для:
    поле ФИО: обязательное, больше 5 символов, меньше 50 символов.
    поле Email: обязательное, тип email
    поле Телефон: обязательное, по возможности использовать паттерн для телефона +38 0ХХ ХХХ-ХХ-ХХ
    поле Дата доставки: необязательное, но если заполнили, то должно быть завтра или послезавтра или после послезавтра.
4. Для валидации даты доставки создать пользовательский валидатор и пользовательскую директиву.
5. При нажатии на кнопку Отправить, выводить в консоль содержимое формы и содержимое корзины в виде объекта:
    { orderId: X,    <- пока номер по порядку (реально должен быть уникальный идентификатор присвоенный на сервере)
      name:          <- значение из поля ФИО
      email:         <- значение из поля Email
      phone:         <- значение из поля Телефон
      ddate:         <- значение из поля Дата доставки или null
      products: []   <- товары корзины
      totalQuantity: <- общее количество
      totalSum:      <- общая сумма
    }