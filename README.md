# Day4_Thousands-seperator

Write a function named format_number that takes a non _negative number as an paramter.
Your function should convert the number to string and add commas as a thousand seperator.

For example calling format_number(1000000) should return "1,000,000".



import json

def format_number():



    a=int(input())

    a=str(a)

    ans=""

    count=1

    l=[]

    b=(a[::-1])

    

    for i in b:

        l.append(i)

        if(count%3==0):

            l.append(",")

        count=count+1

        

    newli=l[::-1]

    if(newli[0]==","):

          newli.remove(newli[0])

    

    for j in newli:

        ans+=j

    print(json.dumps(ans))


format_number()
