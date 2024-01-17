def get_cell_value(dataset, row, column):
    try:
        value = dataset[row][column]
        return value
    except IndexError:
        return "Ячейка не найдена"

while True:
 my_dataset = [
    ['sigma', 18, 'man'],
    ['alex', 46, 'man'],
    ['platon', 13, 'man'],
    ['ivan', 14, 'man']
]

 user_row = int(input("Введите номер строки: "))
 user_column = int(input("Введите номер столбца: "))

 cell_value = get_cell_value(my_dataset, user_row, user_column)
 print("Значение ячейки:", cell_value)
