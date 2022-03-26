from statistics import NormalDist
mu=int(input("Enter the mu"))
sigma=int(input("Enter the sigma"))
dis=NormalDist(mu=mu,sigma=sigma)
print("Enter -1 if you need infinity")
input1=int(input("Enter the input1:"))
input2=int(input("Enter the input2:"))
if(input1==-1 or input2==-1):
    if input1:
        print(0-dis.pdf(input2))
    else:
            print(dis.pdf(input1))
else:
     print(dis.pdf(input2)-dis.pdf(input1))

