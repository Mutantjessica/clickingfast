clickingfast
============

makes you click all fast like for clickingbad
# -*- coding: utf-8 -*-
# <nbformat>3.0</nbformat>

# <codecell>

import time
import win32api, win32con
def click(x,y):
    win32api.SetCursorPos((x,y))
    win32api.mouse_event(win32con.MOUSEEVENTF_LEFTDOWN,x,y,0,0)
    win32api.mouse_event(win32con.MOUSEEVENTF_LEFTUP,x,y,0,0)
  
    

# <codecell>

def play(clicksell=1, clickcook=1, delay=0.01):
    print clicksell, clickcook, delay
    for x in range(clicksell):
        click(150,400)
        time.sleep(delay)
    for x in range(clickcook):    
        click(150, 200)
        time.sleep(delay)

# <codecell>

play(clicksell=1000, clickcook=1500, delay=0.01)

# <codecell>


# <codecell>


# <codecell>


