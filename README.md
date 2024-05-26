# sum_recip_factorial
# The challenge of this task is to be able to produce
# the sum of reciprocals of factorials such as:
# 1 + 1/1! + 2/2! + 3/3! + 4/4! + ...

import math  # So that it would be possible to use the factorial function 

insert_terms = int(input("State the number of terms"))


if insert_terms == 1:
    print("The sum is 1")


else:
    values=[]
    values = [num/math.factorial(num) for num  in range(1 , insert_terms + 1)]
    print(values)
    values_summing = sum(values)
    total = values_summing +1 #adding automatically adds one into the list of values
    print(total)

# How does it work:
# "math" library is imported to use the factorial function
# Next the programm will request a user 
# how many terms the user would like to 
# sum up.
# If just one then the result will be 1
# however if more than one,
# then a list of values ( that is, local variable)
# will be created and subsequently
# the list will be filled up with numbers/factorial of that number
# depending on the range of terms the user required.
# Then the summation will be performed with + 1
# added at the end since it should be added in the beginning.
