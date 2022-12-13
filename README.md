# Broken-Telephone-python
# cook your dish here
for i in range(int(input())):
    n=int(input())
    l=list(map(int,input().split()))
    s=0
    a=False
    for i in range(n-1):
        if l[i]!=l[i+1]:
            s=s+2
            if a:
                s=s-1
            a=True
        else:
            a=False
    print(s)
