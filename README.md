# tv-ligand
import os
os.system ("cls|| clear")

volume= 0
canal= 0

print("Volume: ", volume)
print("Canal: ", canal)
ligar= input("Deseja ligar a TV? (s/n): ")
if ligar == 's':
    tv= print("""TV ligada 
              1- Aumentar volume
              2- Diminuir volume
              3- Aumentar canal
              4- Diminuir canal
              5- Escolher canal
              6- Escolher volume
              7- Desligar TV""")
    opcao= int(input("Digite a opção desejada: "))
else:
    tv= print("TV desligada")     

while opcao != 5:
    if opcao == 1:
        volume= volume + 1
        print("Volume: ", volume)
    elif opcao == 2:
        volume= volume - 1
        print("Volume: ", volume)
    elif opcao == 3:
        canal= canal + 1
        print("Canal: ", canal)
    elif opcao == 4:
        canal= canal - 1
        print("Canal: ", canal)
    elif opcao == 5:
        canal= int(input("Digite o canal desejado: "))
        print("Canal: ", canal)
    elif opcao == 6:
        volume= int(input("Digite o volume desejado: "))
        print("Volume: ", volume)
    elif volume >100:
        print("Volume máximo atingido")
        break
    elif opcao == 7:
        print("TV desligada")
        break
        
    else:
        print("Opção inválida")    
    opcao= int(input("Digite a opção desejada: "))
print("Canal: ", canal)
print("Volume: ", volume)
