#exercicio 1 
def boas_vindas():
    print("Bem-vindo ao mundo das funções!")

boas_vindas()

#exercicio 2 
def saudacao():
    return "Olá, mundo!"

mensagem = saudacao()
print(mensagem)

#exercicio 3
def exibir_nome(nome_aluno):
    print(f"O nome do aluno é: {nome_aluno}")

exibir_nome("Nina")

#exercicio 4
def exibir_numero():
    return "10"
    
numero = exibir_numero()
print(f"{numero}")

#exercicio 5
def exibir_mensagens():
    print("Olá!")
    print("Tudo bem?")
    print("Bom dia!")

exibir_mensagens()

#exercicio 6
def soma(A, B):
   return A + B

resultado = soma(6, 2.9)
print(f"A soma de A e B é: {resultado}")

#exercicio 7
def olá_nome(nome):
    print(f"Olá, {nome}! Seja bem-vindo!")

nome = input("Digite seu nome: ")

olá_nome(nome)

#exercicio 8
def multiplicacao(a, b):
    return a * b

resultado = multiplicacao(6, 10)
print(f"A área do retângulo é: {resultado}")

#exercicio 9
def numero_par_impar(numero):
    if numero % 2 == 0:
        return "par"
    else:
        return "ímpar"

numero = int(input("Digite um número: "))

resultado = numero_par_impar(numero)
print(f"O número é {resultado}")

#exercicio 10
def calcular_media(n1, n2, n3):
    media = (n1 + n2 + n3) / 3
    return media

resultado = calcular_media(9, 8, 7)
print(f"A média é: {resultado}")

#exercicio 11
def numero_maior(n1, n2, n3):
   return max(n1, n2, n3)

resultado = numero_maior(77, 20, 56)
print(f"O maior número é: {resultado}")

#exercicio 12
def temperatura(C):
    F = C * 9/5 + 32
    return F

resultado = temperatura(48)
print(f"48°C é igual a {resultado}°F")

#exercicio 13
def somar_lista(numeros):
    return sum(numeros)

lista = [17, 3.9, 50, 26]
resultado = somar_lista(lista)
print(f"A soma dos números é: {resultado}")

#exercicio 14
def numeros_pares(lista):
    quantidade = 0
    for numero in lista:
        if numero % 2 == 0:
            quantidade += 1
    return quantidade

numeros = [10, 58, 32, 15, 77, 93, 109]
resultado = numeros_pares(numeros)
print(f"A quantidade de números pares é: {resultado}")

#exercicio 15
def potencia(base, expoente):
    resultado = 1
    for _ in range(expoente):
        resultado *= base
    return resultado

print(f"O resultado é: {potencia(2, 3)}")

#exercicio 16
def contar_digitos(numero, digito):
    return str(abs(numero)).count(str(digito))

resultado = contar_digitos(12233334444, 3)
print(f"O dígito 3 aparece {resultado} vezes.")

#exercicio 17
def soma_digitos(numero):
    soma = 0
    for digito in str(abs(numero)):
        soma += int(digito)
    return soma

resultado = soma_digitos(489)
print(f"A soma dos dígitos é: {resultado}")

#exercicio 18
def fatorial(numero):
    if numero < 0:
        return None
    resultado = 1
    for i in range(1, numero + 1):
        resultado *= i
    return resultado

print(fatorial(4))

#exercicio 19
def ordenar_lista(lista):
    lista_ordenada = lista.copy()
    n = len(lista_ordenada)
    
    for i in range(n):
        for j in range(0, n - 1 - i):
            if lista_ordenada[j] > lista_ordenada[j + 1]:

                lista_ordenada[j], lista_ordenada[j + 1] = lista_ordenada[j + 1], lista_ordenada[j]
    
    return lista_ordenada
    
numeros = [20, 67, 38, 93, 42]
ordenada = ordenar_lista(numeros)
print(f"Lista original: {numeros}")
print(f"Lista ordenada: {ordenada}")

#exercicio 20
def inverter(valor):
    return valor[::-1]

print(inverter("python"))
print(inverter([1, 2, 3, 4]))
