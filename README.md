# Insertion-Sort
def Ins(a):
    for i in range(1,len(a)):
        key=a[i]
        j=i-1
        while j>=0 and key<a[j]:
            a[j+1]=a[j]
            j=j-1
        a[j+1]=key
data=[]
n=int(input("How many many Inputs are there : "))
for i in range(n):
    x=float(input("Enter the Input number " +str(i+1)+" : "))
    data.append(x)
Ins(data)
print(data)
