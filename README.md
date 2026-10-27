# hoja_
full_backend

import random
import string

def generate_password(length=12):
    # Объединяем буквы, цифры и знаки препинания
    characters = string.ascii_letters + string.digits + string.punctuation
    # Случайно выбираем символы
    password = ''.join(random.choice(characters) for _ in range(length))
    return password

print("Ваш новый безопасный пароль:")
print(generate_password(16))
