# exercicios

#exercicio01

moeda1cent = int(input('Digite quantas moedas de 1 centavo você tem: '))
moeda5cent = int(input('Digite quantas moedas de 5 centavos você tem: '))
moeda10cent = int(input('Digite quantas moedas de 10 centavos você tem: '))
moeda25cent = int(input('Digite quantas moedas de 25 centavos você tem: '))
moeda50cent = int(input('Digite quantas moedas de 50 centavos você tem: '))
moeda1real = int(input('Digite quantas moedas de 1 real você tem: '))
total = (moeda1cent * 0.01) + (moeda5cent * 0.05) + (moeda10cent * 0.10) + \
        (moeda25cent * 0.25) + (moeda50cent * 0.50) + (moeda1real * 1.00)

print(f'Você tem R${total}')

#exercicio02

tabuada = int(input('Digite um número para ver a sua tabuada: '))
for i in range(1,11):
    print(f'{tabuada} x {i} = {tabuada * i}')

#exercicio03

salario = 1200.00
c1 = 200.00 * 1.02
c2 = 120.00 * 1.02
salariorest = salario - (c1 + c2)

print(f'Vai sobrar R${salariorest:.2f} do salário.')

#exercicio04

a = int(input('Digite o primeiro valor: '))
b = int(input('Digite o segundo valor: '))
if a % b == 0 or b % a == 0:
    print('São múltiplos')
else:
    print('Não são múltiplos')

#exercicio05

n = int(input('Digite o valor de n (1, 2 ou 3): '))
a = int(input('Digite o valor de a: '))
b = int(input('Digite o valor de b: '))
c = int(input('Digite o valor de c: '))

if n == 1:
    print('Valores em ordem crescente:', sorted([a, b, c]))
elif n == 2:
    print('Valores em ordem decrescente:', sorted([a, b, c], reverse=True))
elif n == 3:
    meio = sorted([a, b, c])[1]
    maior = max(a, b, c)
    menor = min(a, b, c)
    print('Valores com o maior no meio:', menor, maior, meio)
else:
    print('Opção inválida')
