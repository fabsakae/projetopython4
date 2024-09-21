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
