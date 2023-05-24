def count_lines(file_path):
    count = 0
    with open(file_path, 'r') as file:
        for line in file:
            count += 1
    return count

def count_empty_lines(file_path):
    count = 0
    with open(file_path, 'r') as file:
        for line in file:
            if line.strip() == '':
                count += 1
    return count

def count_lines_with_z(file_path):
    count = 0
    with open(file_path, 'r') as file:
        for line in file:
            if 'z' in line:
                count += 1
    return count

def count_z_occurrences(file_path):
    count = 0
    with open(file_path, 'r') as file:
        content = file.read()
        count = content.count('z')
    return count

def count_lines_with_and(file_path):
    count = 0
    with open(file_path, 'r') as file:
        for line in file:
            if 'and' in line:
                count += 1
    return count

def print_file_statistics(file_path):
    lines = count_lines(file_path)
    empty_lines = count_empty_lines(file_path)
    lines_with_z = count_lines_with_z(file_path)
    z_occurrences = count_z_occurrences(file_path)
    lines_with_and = count_lines_with_and(file_path)

    print(f"Кількість рядків: {lines}")
    print(f"Кількість порожніх рядків: {empty_lines}")
    print(f"Кількість рядків з літерою 'z': {lines_with_z}")
    print(f"Кількість літер 'z' у файлі: {z_occurrences}")
    print(f"Кількість рядків з групою символів 'and': {lines_with_and}")

# Головний цикл програми
while True:
    file_path = input("Введіть шлях до файлу: ")
    print_file_statistics(file_path)

    choice = input("Бажаєте проаналізувати ще один файл? (Так/Ні): ")
    if choice.lower() != 'так':
        break
