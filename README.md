# calculadorapy
Fiz um speedrun de uma calculadora básica em python, não é suposto ninguém usar, mas fica a vontade, coloquei aqui como forma de salvar isso daqui.


Código:

# Função de soma
def add(a, b):
    return a + b

# Função de subtração
def subtract(a, b):
    return a - b

# Função de multiplicação
def multiply(a, b):
    return a * b

# Função de divisão
def divide(a, b):
    if b == 0:
        return "Erro: divisão por zero não é permitida!"
    else:
        return a / b

# Função principal do programa
def calculator():
    while True:
        print("Selecione uma operação:")
        print("1. Soma")
        print("2. Subtração")
        print("3. Multiplicação")
        print("4. Divisão")
        print("5. Sair")
        choice = input("Digite o número da sua escolha: ")

        if choice == '5':
            print("Encerrando a calculadora...")
            break

        num1 = float(input("Digite o primeiro número: "))
        num2 = float(input("Digite o segundo número: "))

        if choice == '1':
            print("Resultado: ", add(num1, num2))
        elif choice == '2':
            print("Resultado: ", subtract(num1, num2))
        elif choice == '3':
            print("Resultado: ", multiply(num1, num2))
        elif choice == '4':
            print("Resultado: ", divide(num1, num2))
        else:
            print("Escolha inválida. Por favor, tente novamente.")

# Chamar a função principal do programa
calculator()
