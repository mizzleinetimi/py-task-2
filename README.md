import random
import string


while True:

  firstname = input('enter your first name:')
     if len(firstname) <= 0: 
         break
   
   lastname = input('enter your last name:')
    email = input('enter your email address:')


user_details=[]

 user_details = {"firstname":firstname,"lastname":lastname,"email":email}

initials = firstname[0:2] + lastname[-2:]

length=3

random.choice(string.ascii_lowercase) 
a = initials.join (random.choice(string.ascii_lowercase) for i in  range (length))
print ("this is your password:" + a)

print ("is this password okay?")
x = input ("type yes or no")
if x == "yes":
    print (user_details)
     continue

   else:
       print("enter your password")
       password = (input("password should have a numer:"))
       if len(password) <= 7:
           print("your password should be up to 9 characters" )
        password = input("enter password:")
         print(user_details)
 
 else: print(user_details)
    
       
