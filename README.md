# Codigo-da-Transformacao-Python
# ============================================
# 🧩 ATIVIDADES DE PYTHON - OPERAÇÕES BÁSICAS
# ============================================

# 1️⃣ CRIE EXPRESSÕES MATEMÁTICAS USANDO OPERADORES ARITMÉTICOS
print("=== EXERCÍCIO 1: Operadores Aritméticos ===")
n1 = float(input("Digite o primeiro número: "))
n2 = float(input("Digite o segundo número: "))

soma = n1 + n2
subtracao = n1 - n2
multiplicacao = n1 * n2
divisao = n1 / n2
resto = n1 % n2

print(f"\nSoma: {soma}")
print(f"Subtração: {subtracao}")
print(f"Multiplicação: {multiplicacao}")
print(f"Divisão: {divisao}")
print(f"Resto da divisão: {resto}")

# ---------------------------------------------

# 2️⃣ ESCREVA UM PROGRAMA QUE PEÇA DOIS NÚMEROS E MOSTRE QUAL É O MAIOR
print("\n=== EXERCÍCIO 2: Comparar dois números ===")
n1 = int(input("Digite o primeiro número: "))
n2 = int(input("Digite o segundo número: "))

if n1 > n2:
    print(f"O maior número é: {n1}")
elif n2 > n1:
    print(f"O maior número é: {n2}")
else:
    print("Os dois números são iguais.")

# ---------------------------------------------

# 3️⃣ ESTRUTURA IF-ELIF-ELSE PARA CLASSIFICAR IDADE
print("\n=== EXERCÍCIO 3: Classificação por Idade ===")
idade = int(input("Digite sua idade: "))

if idade < 12:
    print("Você é uma criança.")
elif idade < 18:
    print("Você é um adolescente.")
elif idade < 60:
    print("Você é um adulto.")
else:
    print("Você é um idoso.")

# ---------------------------------------------

# 💡 DESAFIO EXTRA: MENU INTERATIVO USANDO WHILE
print("\n=== DESAFIO EXTRA: MENU INTERATIVO ===")

while True:
    print("\nMENU DE OPERAÇÕES:")
    print("1 - Soma")
    print("2 - Subtração")
    print("3 - Multiplicação")
    print("4 - Divisão")
    print("5 - Sair")

    opcao = input("Escolha uma opção (1-5): ")

    if opcao == '5':
        print("Encerrando o programa... Até logo!")
        break

    if opcao in ['1', '2', '3', '4']:
        n1 = float(input("Digite o primeiro número: "))
        n2 = float(input("Digite o segundo número: "))

        if opcao == '1':
            print(f"A soma é: {n1 + n2}")
        elif opcao == '2':
            print(f"A subtração é: {n1 - n2}")
        elif opcao == '3':
            print(f"A multiplicação é: {n1 * n2}")
        elif opcao == '4':
            if n2 != 0:
                print(f"A divisão é: {n1 / n2}")
            else:
                print("Erro: divisão por zero não é permitida.")
    else:
        print("Opção inválida! Tente novamente.")
