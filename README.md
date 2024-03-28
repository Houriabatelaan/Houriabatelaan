commend = ""
started = False
while True:
    commend = input("> ").lower()
    if commend == "start":
       if started:
           print(" Car is already started !")
       else:
           started = True
       print("Car started...")
    elif commend == "stop":
        if not started:
            print("Car is already stopped!")
        else:
         started = False
        print("Car stopped.")
    elif commend == "help":
        print("""
start - to start the car
stop - to stop the car
quit - to quite
        """)
    elif commend == "quit":
        break
    else:
        print("Sorry, I don't understand that")
