# TI BASIC programs
## The Story
These are a few programs I made on my TI calculator in High School, since I had just learned how to code from taking my first computer science class I remember my teacher said TI calculators could be programmed and that's why they aren't allowed in tests, but he never taught us or showed us how. Out of pure interest I took the liberty to learn on my own outside of class. To my surprise I was pretty fluent in TI BASIC, I remember taking my TI calculator everywhere with me and being able to push the buttons non stop. Now looking back at the two programs I have saved it's not as easy to understand as I would have years ago, but still understandable. Sadly there are other programs that have gone missing because I accidentally forgot my TI calculator under my desk when taking a test.

I remember there was a high low program where the computer had to guess the user's number and in the end told the user how many tries it took to guess the number. Another program I remembered was the called "Graph" and soon I created my first GUI program based of this idea for my first computer science class which can be seen [here](https://github.com/ImaginaryResources/Connecting-Dots)

I could recreate the programs I lost easily, but because it wasn't created by the true drive I had in the beginning I feel like it would be ingenue to recreate them. In fact I was going to, but it felt like a chore. I want to document this moment because this was the first time I took something out of class and ever since this moment I have kept going, this was the inital push for my love of computer science.

## Guess The Number
The calculator generates a random number and the user has to guess it with one try
```
ClrHome
Disp "GUESS A NUMBER"
0→B
Input "[1-50]:",C
randInt(1,50)→B
If B≠C:Then
Disp "SORRY"
Else
Disp "WINNER"
End
Disp "THE NUMBER WAS",B
"
```
This seems impossible but I remember being so excited that I took this very picture on 1/8/16
<img src="https://github.com/ImaginaryResources/TI-BASIC-programs/blob/master/Winner.png" width="300">

## Cookie Game
This was a [Cookie Clicker](http://orteil.dashnet.org/cookieclicker/) inspired game and was just as addictive, for me. I'm glad this program was saved because this was one of the best ones I made, so I'm glad it survived. I never got the mathematics for this program right to have a nice progression, but I remember writing out exponential equations for this program and trying to find the best configuration 

The user just needs to continuously tap "1" to gain points by one and when a certain amount of points are accumulated then button two is unlocked and the user can now tap "2" to gain points by two, so on and so forth. Tapping a button that is locked will tell the user it's locked and how many points are required to unlock it
```
ClrHome
Disp "PRESS A NUMBER"
Disp "KEY FOR MONEY"
Disp "(CLEAR=EXIT)"
0→A
0→D
For(C,0,100000)

Repeat B=92
Repeat B=93
Repeat B=94

Repeat B=82
Repeat B=83
Repeat B=84

Repeat B=72
Repeat B=73
Repeat B=74

Repeat B=102
Repeat B=103

Repeat B=45
getKey→B

If B=92:Then
A+1→A
D+1→D
Disp "+1"
Disp A
If A≥200:Then
Disp "+2 UNLOCKED"
Disp "CLICK 2"
End

Else
If B=93 and A≥200:Then
A+2→A
D+1→D
Disp "+2"
Disp A
If A≥500:Then
Disp "+3 UNLOCKED"
Disp "CLICK 3"
End

Else
If B=94 and A≥500:Then
A+3→A
D+1→D
Disp "+3"
Disp A
If A≥1000:Then
Disp "+4 UNLOCKED"
Disp "CLICK 4"
End

Else
If B=82 and A≥1000:Then
A+4→A
D+1→D
Disp "+4"
Disp A
If A≥2000:Then
Disp "+5 UNLOCKED"
Disp "CLICK 5"
End

Else
If B=83 and A≥2000:Then
A+5→A
D+1→D
Disp "+5"
Disp A
If A≥5000:Then
Disp "+6 UNLOCKED"
Disp "CLICK 6"
End

Else
If B=84 and A≥5000:Then
A+6→A
D+1→D
Disp "+6"
Disp A
If A≥10000:Then
Disp "+7 UNLOCKED"
Disp "CLICK 7"
End

Else
If B=72 and A≥10000:Then
A+7→A
D+1→D
Disp "+7"
Disp A
If A≥15000:Then
Disp "+8 UNLOCKED"
Disp "CLICK 8"
End

Else
If B=73 and A≥15000:Then
A+8→A
D+1→D
Disp "+8"
Disp A
If A≥25000:Then
Disp "+9 UNLOCKED"
Disp "CLICK 9"
End

Else
If B=74 and A≥25000:Then
A+9→A
D+1→D
Disp "+9"
Disp A
If A≥50000:Then
Disp "+10 UNLOCKED"
Disp "CLICK 10"
End

Else
If B=102 and A≥50000:Then
A+10→A
D+1→D
Disp "+10"
Disp A

Else
If B=93 and A≤200:Then
Disp "+2 LOCKED"
Disp "200+ TO UNLOCK"

Else
If B=94 and A≤500:Then
Disp "+3 LOCKED"
Disp "500+ TO UNLOCK"

Else
If B=82 and A≤1000:Then
Disp "+4 LOCKED"
Disp "1000+ TO UNLOCK"

Else
If B=83 and A≤2000:Then
Disp "+5 LOCKED"
Disp "2000+ TO UNLOCK"

Else
If B=84 and A≤5000:Then
Disp "+6 LOCKED"
Disp "5000+ TO UNLOCK"

Else
If B=72 and A≤10000:Then
Disp "+7 LOCKED"
Disp "10000+ TOUNLOCK"

Else
If B=73 and A≤15000:Then
Disp "+8 LOCKED"
Disp "15000+ TO UNLOCK"

Else
If B=74 and A≤25000:Then
Disp "+9 LOCKED"
Disp "25000+ TO UNLOCK"

Else
If B=102 and A≤50000:Then
Disp "+10 LOCKED"
Disp "50000+ TO UNLOCK"

Else
If A=100000:Then
Disp "WINNER"
Stop

Else
If B=103:Then
Disp "TOTAL CLICKS",D

Else
If B=45:Then
Disp "TOTAL CLICKS",D
Stop

End
End
End
End
End
End
End
End
End

End
End
End
End
End
End
End
End
End
End
End
End
End
End
"
```

