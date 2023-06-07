Olá esse projeto ensina você usar o Git
Isso é uma alteração

import time 
suspeito = [str.upper(input('Para quem você se dirige primeiro? '))]

def escolher ():
    while suspeito != "ALICE" or suspeito != "LUCAS" or suspeito != "PIETRO" or suspeito != "CARMEN":
        print('Resposta inválida')
        suspeito = [str.upper(input('Para quem você se dirige primeiro? '))]

        escolher()
    
    if suspeito == ['ALICE']:
        print('Você interroga Alice.') 
        time.sleep(3)
        print('Ela começa a chorar, te questionando o porquê de você suspeitar dela, e diz que só queria um final de semana em paz com os amigos.')
        time.sleep(3)
        suspeito.pop("ALICE")
        
    elif suspeito == 'LUCAS':
        print('Você interroga Lucas.')
        time.sleep(3)
        print('Ele começa a te xingar de tudo que é nome, e diz que você é um idiota por achar que ele é o assasino.')
        time.sleep(3)
        
    elif suspeito == 'CARMEN':
        print('Você interroga Carmen.')
        time.sleep(3)
        print('Ela diz que seria impossível, porque ela possui uma grande intimidade com todo o grupo.')
        time.sleep(3)
        
    elif suspeito == 'PIETRO':
        print('Você interroga Pietro.')
        time.sleep(3)
        print('Pietro se desespera mais ainda, com medo de ser o próximo, e afirma à você que não foi ele.')
        time.sleep(3)
        
    escolher()
suspeito = input('Qual será o próximo a ser interrogado? ')
escolher()
suspeito = input('Qual será o próximo a ser interrogado? ')
escolher()
suspeito = input('E por último: ')
escolher()
