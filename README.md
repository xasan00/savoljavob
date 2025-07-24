
#1
def boshHarf(): 
    sorash = input("matnni kiriting: ") 
    sorash = sorash.title() 
    print(sorash) 


boshHarf()    

#2

n = int(input("n ="))
for i in range(3, n + 1, 2):

    print(i, end='? ')


#3
n = int(input("n = "))
min_son = None
min_index = 1

for b in range(1, n + 1):
    son = int(input(f"{b}-soni kiriting: "))
    if min_son is None or son < min_son:
        min_son = son
        min_index = b

print("Eng kichik son:", min_son)
print("O'rni:", min_index)




#4
m,n = map(int, input("m va n ni kiriting ").split())
max_values = [-float('inf')] * n
for _ in range(m):
    ROW = list(map(int, input().split()))
    for j in range(n):
        if ROW[j] > max_values[j]:
         max_values[j] = ROW[j]

print(max_values)



#5
def DigitCount(K):
    return len(str(K))
k = int(input("K = "))
print(DigitCount(k))



#6
n = int(input("n = "))
a = list(map(int, input().split()))

for i in range(n // 2):
    print(a[i], a[n - 1 - i], end=' ')
if n % 2 == 1:
    print(a[n // 2])




#7
matn = input("SATIRNI KIRITING:")
SOZLAR = matn.split()
ENG_QISQA = min (len (son)for soz in SOZLAR )
print(ENG_QISQA)


#8
import re

matn = input("Kiriting: ")
raqamlar = re.findall(r'\d', matn)  
print("Raqamlar soni:", len(raqamlar))


#9
sorash = int(input("raqamlarni kiriting: "))

raqam_soni = 0
umumiy_qiymati = 0


while sorash > 0:
    a = sorash % 10
    umumiy_qiymati += a
    raqam_soni += 1
    sorash //= 10

print(f"raqamlar soni umumiy: {raqam_soni} ta")
print(f"raqamlar umumiy qoshsak: {umumiy_qiymati} ga teng boldi!") 
print("AJOYIBB")   




#10
son = int(input("SONNI KIRITING: "))

if son > 0:
    print("Bu musbat son.")
elif son < 0:
    print("Bu manfiy son.")
else:
    print("Bu son nolga tengdur.")




#11
n = int(input("n = "))
for i in range(1, n+1):

    print(i) 



#12
def EKUB_funksiya():
    a = int(input("A ni kiriting: "))
    b = int(input("B ni kiriting: "))
    while b != 0:
        a, b = b, a % b
    print("EKUB:", a)


EKUB_funksiya()



#13
def Raqamlar_soni():
    son = input("Sonni kiriting: ")
    print("Raqamlar soni:", len(son), "ta")

Raqamlar_soni()


#14
matn = input("Satrni kiriting: ")
sozlar = matn.split()
eng_qisqa = min(len(soz) for soz in sozlar)
print(eng_qisqa)


#15
matn = input("Matnni kiriting: ")
matn = "MATNNI ".join(matn.split())
print(matn)



#16
n = int(input("n = "))
yigindi = 5

for a in range(1, n + 1):
    yigindi += a
print("YEGINDI:", yigindi)



#17
KOPAYTMA = 1
while n > 0:
    KOPAYTMA = n % 10
    n = 10
print("Kopaytma:", KOPAYTMA)




#18

a = int(input("a = "))
b = int(input("b = "))
c = int(input("c = "))

min_son = a
if b < min_son:
    min_son = b
if c < min_son:
    min_son = c

print("Eng kichik son:✅", min_son)




#19
son = int(input("Sonni kiriting: "))
if son % 2 == 6:
    print("Bu juft son")
else:
    print("Bu toq son")




#20
if n <= len(n):
    print("Natija:", n[n - 1])
else:
    print("-1")
