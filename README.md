# projetopython4
# Cálculo de média

    num1 = float(input('Digite o primeira nota: '))
    num2 = float(input('Digite o segunda nota: '))
    media = (num1 + num2) / 2
    print('A primeira nota foi {:.1f}, a segunda nota foi {:.1f} e A sua MÉDIA é: {:.1f} '.format(num1, num2, media))
    if media >= 5 and media < 7:
        print('Você está em RECUPERAÇÃO.')
    elif media < 5:
        print('Você está REPROVADO.')
    else:
        print('Você está APROVADO!')

# Identificador de triângulos

    reta1 = float(input('Digite o primeiro segmento da reta: '))
    reta2 = float(input('Digite o segundo segmento da reta: '))
    reta3 = float(input('Digite o terceiro segmento da reta: '))
    if reta1 < reta2 + reta3 and reta2 < reta1 + reta3 and reta3 < reta1 + reta2:

        if (reta1 == reta2) and (reta1 == reta3) :
                print('Equilatero')
        elif (reta1 == reta2) or (reta1 == reta2) or (reta2 == reta3):
                print('Isósceles')
        else:
                print('Escaleno')
    else:
        print('Não formam um triângulo')

# calculadora de IMC

    peso = float(input('Digite seu peso (Kg): '))
    altura = float(input('Digite sua altura (m): '))
    imc = peso / (altura ** 2)
    print('Seu Índice de massa corporal é: {:.1f} ! '.format(imc), end='')

    if imc <= 18.5:
    print('Você está abaixo do peso!')
    elif imc <= 25:
        print('Você está com seu peso Ideal!')
    elif imc <= 30:
        print('Você está com Sobrepeso!')
    elif imc <= 40:
        print('Você está Obeso!')
    else:
        print('Você está com obesidade Morbida, Procure ajuda médica!')

# Calculadora de descontos
    print('{:=^40}'.format(' LOJAS TKG '))
    valor = float(input('Total das Compras (R$): '))
    print('''FORMAS DE PAGAMENTO
    [ 1 ] à vista/PIX
    [ 2 ] débito
    [ 3 ] 2 X cartão
    [ 4 ] 3 X ou mais no cartão ''')
    opção = int(input('Qual sua opção? '))
    if opção == 1:
        total = valor - (valor * 10 / 100)
    elif opção == 2:
        total = valor - (valor * 5 / 100)
    elif opção == 3:
        total = valor
        parcela = total / 2
        print('Sua compra será parcelada em 2x sem juros de R$ {:.2f}'.format(parcela))
    elif opção == 4:
        total = valor + (valor * 20 /100)
        totalparc = int(input('Quantas parcelas? '))
        parcela = total / totalparc
        print('sua compra será parcelada com juros em {}x de R$ {:.2f}'.format(totalparc, parcela))
    else:
        total = valor
        print('Opção inválida. Digite novamente!')
    print('sua compra de R$ {:.2f} ficará por {:.2f}'.format(valor, total))
