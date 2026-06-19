# Projeto simples:
# Cadastra alunos e notas em um arquivo CSV.
# Depois lê o arquivo e calcula:
# - média da turma
# - maior nota
# - menor nota

alunos = []

while True:
    nome = input('Digite o nome do aluno: ')

    if nome == '0':
        break

    nota = float(input('Digite a nota do aluno: '))


    alunos.append((nome,nota))

with open('alunos.csv', 'w') as arquivo:
    arquivo.write('nome,nota \n')

    for name,grade in alunos:
        arquivo.write(f'{name},{grade}\n')

with open('alunos.csv', 'r') as arquivo:
    next(arquivo)

    soma = 0
    contador = 0	
    menor = 11
    menor_nome = '0'
    maior = 0
    maior_nome = '0'
    for linha in arquivo:
        nome,nota = linha.strip().split(',')
        nota = float(nota)
        soma  +=nota
        contador +=1
    
        if nota > maior:
            maior = nota
            maior_nome = nome

        if nota < menor:
            menor = nota
            menor_nome = nome    


    media = soma/contador

    print(f'A media dos alunos foi de {media}')

    print(f'O aluno {maior_nome} teve a maior nota {maior}')

    print(f'O aluno {menor_nome} teve a menor nota {menor}')
