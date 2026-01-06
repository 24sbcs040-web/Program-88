# Sum of digits until it reduces to single digit

# Reading number
number = int(input("Enter number: "))

# Finding sum
total_sum = 0
step = 1

condition = True

while condition:
    while number:
        total_sum += number % 10
        number //= 10

    print("Step-%d Sum: %d" % (step, total_sum))
    number = total_sum
    total_sum = 0
    step += 1
    condition = number > 9

output:
Enter number: 5446
Step-1 Sum: 19
Step-2 Sum: 10
Step-3 Sum: 1
