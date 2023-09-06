import random

options = ("piedra", "papel", "tijera")

computer_win = 0
user_win = 0
round = 1
while True:
  print('*' * 15)
  print('ROUND', round)
  print('*' * 15)
  print('Humano', user_win)
  print('Maquina', computer_win)

  user_option = input("piedra, papel o tijera => ")
  user_option = user_option.lower()
  round += 1
  if not user_option in options:
    print("Esa opción no es valida")
    continue

  computer_option = random.choice(options)

  print("Tu opcion => ", user_option)
  print("Opcion de la maquina => ", computer_option)
  if user_option == computer_option:
    print("empate")
  elif user_option == "piedra":
    if computer_option == "tijera":
      print("piedra gana a tijera")
      print("Ganaste!")
      user_win += 1
    else:
      print("papel gana a piedra")
      print("la maquina gana")
      computer_win += 1
  elif user_option == "papel":
    if computer_option == "piedra":
      print("papel gana a piedra")
      print("Ganaste!")
      user_win += 1
    else:
      print("tijera gana a papel")
      print("la maquina gana")
      computer_win += 1
  elif user_option == "tijera":
    if computer_option == "papel":
      print("tijera gana a papel")
      print("Ganaste!")
      user_win += 1
    else:
      print("piedra gana a tijera")
      print("la maquina gana")
      computer_win += 1
  if computer_win == 3:
    print('El rotundo ganador es la maquina')
    break
  if user_win == 3:
    print('Eres el rotundo ganador')
    break
