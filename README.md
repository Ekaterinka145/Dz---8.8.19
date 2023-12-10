amount = 0
tickets = int(input("Введите количество билетов:\n" ))
for value in range(tickets):
    age = int(input("Введите возраст посетителя:\n" ))
    if age < 18:
        amount += 0
        print("Проходите бесплатно")
        print("Сумма покупки", amount, "руб.")
    elif age >= 18 and age <= 25:
        amount += 990
        print("Сумма покупки", amount, "руб.")
    elif age > 25:
        amount += 1390
        print("Сумма покупки", amount, "руб.")
    else:
        print("Кол-во билетов:", tickets, "шт." )
    if tickets > 3 :
        discount = amount / 100 * 10
        print("Скидка составляет:",discount, "руб.")
        print("Итоговая оплата с учетом скидки:",(amount -discount), "руб.")
