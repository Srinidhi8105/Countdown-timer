# Countdown-timer
Built a countdown timer using python's time library
import time
def countdown(t):
    while t:
        mins,secs=divmod(t,60)
        timer='{:02d}:{:02d}'.format(mins,secs)
        print(timer,end="\r")
        time.sleep(1)
        t-=1
    print("fire in the hole")

t=int(input("enter time in seconds: "))
countdown(t)
