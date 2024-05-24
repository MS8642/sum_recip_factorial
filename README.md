# sum_recip_factorial

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
