# projetopython4
estudo python
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
