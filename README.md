# water-calculator
it is a water calculator that tells you how much water should you drink based on your height and weight
'''Hi!
  My program calculates: How much water should an adult drink per day ???
  To do this, enter the following:
Weight: sample ( 70 )
Height: sample ( 170 )
                                           '''
m = int(input('Your weight: ',))
print(m,'kg ✓')
h = int(input('Your height: ',))
print(h,'sm ✓')

w = "🔘Potable Water  — "
fl = "🟢Total(🍵+🍹+🥛) —"
mi = h - 100
fn = mi*30/1000
fd = mi*40/1000
wn = round(fn*0.6, 1)
gn = round(wn/0.22)*'🥛'
if m <= mi:
  print(w,wn,'liter =',gn)
  print(fl,round(fn,1),"liter")
elif m > mi:
  print('''  If you are overweight and want to lose weight, then:''')
  wd = round(fd*0.6, 1)
  gd = round(wd/0.22)*'🥛'
  print(w,wd,'liter =',gd)
  print(fl,round(fd,1),'liter')
  print('''  
  And if you don't want to lose weight,then:''')
  print(w,wn,'liter =',gn)
  print(fl,round(fn,1),"liter")

print('''
1🥛 =  200-250 ml
———————————————————————————————————————————>
  Water is the basis of human life
The human body consists of 60-70% water. Interestingly, the embryo in the fifth month of life in the womb consists of 94% water. But the human body is designed in such a way that it loses moisture with age. With age, the water saturation coefficient already becomes 85-70%.
  It is necessary to observe a drinking regime throughout life. To avoid unpleasant symptoms such as fatigue, lethargy, irritability, increased blood pressure and other indicators. Bringing the consumption of clean water to the required norm increases life expectancy by an average of 15-20 years''')


