# Recursividad



def torres_de_hanoi(n, origen, destino, auxiliar):
  
  if n == 1:
   
    print(f"Mover disco 1 de {origen} a {destino}")
  
  else:
    
    torres_de_hanoi(n-1, origen, auxiliar, destino)
    print(f"Mover disco {n} de {origen} a {destino}")
    torres_de_hanoi(n-1, auxiliar, destino, origen)

numero_discos = 3

torres_de_hanoi(numero_discos, "A", "C", "B")
