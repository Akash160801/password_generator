# password_generator

You can generate a strong password for your accounts of desired length.

import string 

import random

if __name__ =="__main__":


  s1=string.ascii_lowercase 
  
  s2=string.ascii_uppercase
  
  s3=string.digits
  
  s4=string.punctuation
  
  
  # int is used to convert the input into integer.
  

  ps_len = int (input("Enter the password length:"))  
  
  s=[]
  
  
  # to convert string into list , we are using list constructor.
  
  
  s.extend(list(s1)) 
  
  s.extend(list(s2))
  
  s.extend(list(s3))
  
  s.extend(list(s4))
  
  
  #to shuffle the strings.
  
 
  random.shuffle(s) 
  
  print("Your password is:")
  
  
  #join is used to concatenate the elemnts of the string.
  
  
  print("".join(s[0:ps_len]))   
