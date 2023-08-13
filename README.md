# txt12
ded
N = int(input())
number = N
def join(lst):
    return ''.join(map(str, lst))
while True:
  mylist = []
  mylist_1 = []
  for digit in str(number):
     mylist.append(digit)
  for i in range(len(mylist)):
    mylist_1.append(mylist[len(mylist)-1-i])
  if mylist == mylist_1:
     num = join(mylist)
     print(num)
     break
  else:
     num_1 = int(join(mylist))
     num_2 = int(join(mylist_1))
     number = num_1 + num_2
