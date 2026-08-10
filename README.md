# My-Own-AI-App-Launcher
#My program can open any app present in a system. If the app is not downloaded in that system, it will simply opens App Store for you. #It contains a secret code of 3 digits for enabling the access to the program. It also opens apps in web browsers but for that, the secret code is made different... 

def ai():
    
    a= 100
    b= 200
    n= int(input("Enter three digit secret code: "))
    if (n==a):
        print("Access AI Successfully")
        n= input("What is your name? ")
        print(f"Hello, {n}  Sir")
        import os

        c= input("What you want to open? ").lower()
        result= os.system("open -c'" + c + "'")

        if result!=0:
            print("App Not Found")
            os.system("open -c 'App Store'")
        
    elif (n==b):
        print("Access AI Successfully")
        n= input("What is your name? ")
        print(f"Hello, {n}  Sir")
        import os
        
        d= input("Want to open any application in browser? ")
        os.system("open -u 'https://" + d +".com'")

        
    else:
        print("Access Denied")

ai()
        
        
       
        

        
        

       
           
      

        
    
        
