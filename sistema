saldo=500.00
saque_diario=3
saques_realizados=0
opcao=0
saques=[]
depositos=[]
while (opcao!=4):
   

   opcao=int(input
          ("""Informe uma opção: 
[1] Sacar 
[2] Depositar 
[3] Extrato 
[4] Sair 
"""))


   if (opcao==1):
       
       valor=float(input("Digite o valor do saque: "))
       if(valor>saldo):
          print("Saldo insuficiente")
       elif(valor > 500):
           print("Limite de valor exedido")
       elif(saques_realizados>= saque_diario):
           print("Limite de saque exedido")
       else:
          saldo -= valor
          saques_realizados += 1
          saques.append(valor)
          print(f"Saque de R${valor:.2f} foi realizado com sucesso!")
          print(f"Saldo restante: R${saldo:.2f}",)
          
   elif (opcao==2):
      valor=float(input("Digite o valor do deposito: "))
      saldo += valor
      depositos.append(valor)
      print(f"O depósito de R${valor:.2f} foi realizado com sucesso!")
      print(f"Saldo atual: R${saldo:.2f}")
      
   elif (opcao==3):
      print("Extrato: ")
      if depositos:
         depositos_str = ', '.join(f'R${d:.2f}' for d in depositos)
         print(f"Depósitos: R${depositos_str}")
      else:
         print("Depósitos: R$0.00") 
      if saques:
            saques_str = ', '.join(f'R${s:.2f}' for s in saques)
            print(f"Saques: {saques_str}")
      else:
            print("Saques: R$0.00")
      print(f"saldo atual: R${saldo:.2f}")
      print(f"Saques realizados hoje:{saques_realizados}/{saque_diario}")
   
   elif (opcao==4):
      print("Saindo do sistema bancário...")

   else: 
      print("Opção inválida. Escolha uma opção válida")
      print()

      print("Sistema bancário encerrado.")
