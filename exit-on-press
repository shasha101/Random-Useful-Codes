from pynput import keyboard
import time
break_program = False
def on_press(key):
    global break_program
    print (key)
    if key == keyboard.Key.end:
        print ('end pressed')
        break_program = True
        return False
with keyboard.Listener(on_press=on_press) as listener:
    while break_program == False:
        print ('program running')
        time.sleep(5)
    listener.join()
