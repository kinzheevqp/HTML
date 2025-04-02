import random
import string

def generate_passwords(full_name, birth_date):
    # Создаем уникальные начальные элементы на основе ФИО и даты рождения
    base = full_name.lower() + birth_date.replace("-", "")

    # Символы для добавления в пароли
    special_chars = "@*#!$%^&*"

    passwords = []

    for i in range(10):
        # Генерируем уникальный пароль, перемешивая части строки
        random_str = ''.join(random.choices(string.ascii_lowercase + string.digits + special_chars, k=5))
        password = base + random_str
        passwords.append(password)

    return passwords


def main():
    # Ввод ФИО и даты рождения
    full_name = input("Введите ваше ФИО: ")
    birth_date = input("Введите вашу дату рождения (в формате ГГГГ-ММ-ДД): ")

    # Генерация паролей
    passwords = generate_passwords(full_name, birth_date)

    # Выводим 10 уникальных паролей
    print("\nСгенерированные пароли:")
    for password in passwords:
        print(password)


if __name__ == "__main__":
    main()
