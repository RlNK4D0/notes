#programacion 
```
 estacion = input("ingrese la estacion: ")
 lugar = input("ingrese el destino: ")

 match estacion : 
	 case "invierno":
		 if lugar == "bariloche"
			 print(" ")
	 
	 case "verano":
		 match lugar:
			 case "mdp":
				 print("")
			 case "cataratas"
				 print("")
			 case "bariloche"
				 print("")
				 
	 case "otoño":
		 if condicion:
			 print("")
	 case "primavera":
		 if condicion:
			 print("")
	 case_:
		 caso por defecto (basicamente el else del if)
```

**match** ==ÚNICAMENTE== pregunta por igualdad ``==``
Los match pueden **anidarse** al igual que los if
