
palavra = (input("Escreve uma palavra: "))
palavra_descoberta=["_"]*len(palavra)
tamanho_palavra= len(palavra)

erros=0
max_tentativas=7
conj_letras_certas=set()
conj_letras_pedidas=set()
fimJogo=False

print(palavra_descoberta)
total_letras_certas=0
while not fimJogo:
  letra=input("Escreve uma letra: ")
  if letra in conj_letras_pedidas:
    print("Essa letra já foi pedida")
  else:
    conj_letras_pedidas.add(letra)
    for i in range(tamanho_palavra):
      if palavra[i] == letra:
        palavra_descoberta[i]=letra
        total_letras_certas+=1

  if erros == 1:
    print(" |---------------")
    print(" |              |")
    print(" |              O")
    print(" |")
    print(" |")
    print(" |")
    print("_|_")
  if erros == 2:
    print(" |---------------")
    print(" |              |")
    print(" |              O")
    print(" |              |")
    print(" |              |")
    print(" |")
    print("_|_")
  if erros == 3:
    print(" |---------------")
    print(" |              |")
    print(" |              O")
    print(" |             /|")
    print(" |              |")
    print(" |")
    print("_|_")
  if erros == 4:
    print(" |---------------")
    print(" |              |")
    print(" |              O")
    print(" |             /|\ ")
    print(" |              |")
    print(" |")
    print("_|_")
  if erros == 5:
    print(" |---------------")
    print(" |              |")
    print(" |              O")
    print(" |             /|\ ")
    print(" |              |")
    print(" |             / ")
    print("_|_")
  if erros == 6:
    print(" |---------------")
    print(" |              |")
    print(" |              O")
    print(" |             /|\ ")
    print(" |              |")
    print(" |             / \ ")
    print("_|_")

  if total_letras_certas == tamanho_palavra:
    fimJogo=True
    print("Ganhas-te")
  if letra not in palavra:
    erros+=1
  if erros == max_tentativas:
    print("Perdes-te")
    fimJogo=True

  print(palavra_descoberta)
  print("letras saidas:",conj_letras_pedidas, "certas:", total_letras_certas, "erros", erros)
