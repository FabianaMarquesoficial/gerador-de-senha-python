# gerador_senhas.py

import random
import string

def gerar_senha(tamanho=12):
    caracteres = string.ascii_letters + string.digits + string.punctuation
    senha = ''.join(random.choice(caracteres) for _ in range(tamanho))
    return senha

if __name__ == "__main__":
    try:
        tamanho = int(input("Digite o comprimento da senha: "))
        senha = gerar_senha(tamanho)
        print(f"Senha gerada: {senha}")
    except ValueError:
        print("Por favor, insira um número inteiro válido.")
        
- [Site oficial do Python](https://www.python.org/) — Baixe o Python, leia a documentação e explore tutoriais.
