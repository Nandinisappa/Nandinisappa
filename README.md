
oil=180
flour=150
spices=100
drinks=50
chips=50
cname=input('enter customer name: ')
cnum=input('enter customer phone number: ')
oq=int(input('enter no of oil packets: '))
fq=int(input('enter no of flour packets: '))
sq=int(input('enter no of spices packets: '))
dq=int(input('enter no of  drinks packets: '))
cq=int(input('enter no of chips packets: '))
bill=(oil*oq)+(flour*fq)+(spices*sq)+(drinks*dq)+(chips*cq)
if bill>=5000:
      dis=bill*10/100
      tax=0
if bill>=3000:
     dis=bill*8/100
     tax=0
elif bill>=2000:
     dis=bill*5/100
     if bill>=1000:
         dis=bill*3/100
         if bill>=3000:
             tax=bill*10/100
else:
     tax=bill*18/100
mainbill=bill-dis+tax
print('bill amount: ', mainbill)
