def soma(a,b):
  return a + b

def subtracao(a,b):
  return a - b

def multi(a,b):
  return a * b

def divisao(a,b):
  if b == 0:
    return 'Erro'
  else:  
    return a / b

while True: 

  operacao = input('Digite a operação que quer realizar: soma/subtracao/multiplicacao/divisao. Ou digite 0 para encerrar.').lower()

  if operacao == "0":
    break
  elif operacao != "soma" and operacao != "subtracao" and operacao != "multiplicacao" and operacao != "divisao":
    print("Erro, digite uma operacação valida.") 
    continue  

  num1 = int(input('Digite o primeiro número: '))
  num2 = int(input('Digite o segundo número: '))


  if operacao == "soma":
    print(soma(num1,num2))
  elif operacao == "subtracao":
    print(subtracao(num1,num2))
  elif operacao == "multiplicacao":
    print(multi(num1,num2))
  elif operacao == "divisao":
    print(divisao(num1,num2))  
