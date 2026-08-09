# My-Own-AI-App-Launcher
#My program can open any app present in a system. If the app is not downloaded in that system, it will simply opens App Store for you. #It contains a secret code of 3 digits for enabling the access to the program...
def ai():
    
    a= 100
    n= int(input("Enter three digit secret code: "))
    if (n==a):
        print("Access AI Successfully")
        n= input("What is your name? ")
        print(f"Hello, {n}  Sir")
        import os

        a= input("What you want to open? ").lower()
        result= os.system("open -a'" + a + "'")

        if result!=0:
            print("App Not Found")
            os.system("open -a 'App Store'")

        
    else:
        print("Access Denied")

ai()
