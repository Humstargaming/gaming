1.saturs
    datoram ir jagenere skaitlis no 1-100
    cikveks megina uzminet skaitli kamer dators saka mazak vai vairak




```py
import random

repeat = True


while repeat:
    number = random.randint(1, 100)
    guess = 0
    tries = 0
    while guess != number:
        guess = int(input("Uzmini skaitli: "))
        if number < guess:
            tries+=1 
            print("mazak")
        elif number > guess:
            tries+=1
            print("vairak")
        else:
            if tries < 4:
                print(f"WOW! uzminēji tikai pēc {tries} reizēm!")
            elif tries < 7:
                print(f"Nav slikti, uzminēji pēc {tries} reizēm!")
            else:
                print(f"Hm... vajadzētu patrenēties, uzminēji pēc {tries} reizēm!")
    
    atbilde = input("vai gribi atkartot y/n: ")
    if atbilde == "y":
        repeat = True
    elif atbilde == "n":
        repeat = False
        print("ata")
    else:
        repeat = False
        print("ata")

```
