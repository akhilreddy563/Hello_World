# Hello_World
#FLAMES Game using Python language
import string
p1=input("Enter a first person name :")
p1=p1.lower()
p1=p1.replace(" ","")

p2=input("Enter a second person name :")
p2=p2.lower()
p2=p2.replace(" ","")

l1=list(p1)
l2=list(p2)

def removing_matching_letters(l1,l2):
    for i in range(len(l1)):
        for j in range(len(l2)):
            if l1[i]==l2[j]:
                c=l1[i]
                l1=l1.remove(c)
                l2=l2.remove(c)
                l=l1+[*]+l2
                return True
    l=l1+['*']+l2
    return False

proceed=True
while proceed:
    ret_list=removing_matching_letters(l1,l2)
    cont_list=ret_list[0]
    cont_list=ret_list[1]
    
        
	
	
    
    


