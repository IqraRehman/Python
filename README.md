# Python
Practice Programs

Q#1:Write a function called city_country() that takes in the nameof a city and its country. The function should return a string formatted like this:"Santiago, Chile"Call your function with at least three city-country pairs, and print thevalues that are returned.

def city_country(country, city):
    return country + ", " + city

print(city_country("Pakistan", "Islamabad"))
print(city_country("Austraila", "Sydney"))
print(city_country("America", "NewYork"))

Q#2:Write a function called make_shirt() that accepts a size and thetext of a message that should be printed on the shirt. The function should printa sentence summarizing the size of the shirt and the message printed on it.Call the function once using positional argumentsto make a shirt. Call the function a second time using keyword arguments.

def make_shirt(shirt_size, message):
    print(f"The size of the shirt is {shirt_size}")
    print(f"It will say {message}")

shirt_size = int(input("Enter size of shirt(small, Medium, Large): "))
message = input("Enter message: ")
make_shirt(shirt_size, message)
make_shirt(shirt_size = "Medium", message = "I Love My Life")

Q#3:Write a function called describe_city() that accepts the name ofa city and its country. The function should print a simple sentence, such as Reykjavik is in Iceland. Give the parameter for the country a default value.Call your function for three different cities, at least one of which is not in the default country.

def describe_city(city, country='Pakistan'):
    print(f"{city} is in {country}.")

describe_city('Islamabad')
describe_city('Melbourine')
describe_city('Saudia', 'Makkah')

Q#4:Make a function to find factorials of given number

def factorial(number):
    fact = 1
    for i in range(1,number+1):
        fact *= i
    print(fact)
        
factorial(4)

Q#5:function to find Faboocii series till given Number

def fibonacci(number):
    a = 1
    b = 1
    print("Fibonacci series")
    print(a, b, end = " ")
    for i in range(1, number+1):
        cur = a + b
        a = b
        b = cur
        print(cur, end = " ")
num = int(input("Enter Ending point: "))
fibonacci(num)

Q#6:function to print pair prime numbers till given input number

def prime_numbers(number):
    for num in range(2, number+1):
        if num > 1:
           for i in range(2, num):
                if (num % i) == 0:
                    break
           else:
                print(num)
num = int(input("Enter limit: "))         
prime_numbers(num)

Q#7:Make a function, that takes a list as argument, return a list of square of each elements in the argument lists and finally prints both lists.

def func(list):
    square = []
    for i in list:
        square.append(i*i)
    return square

n = int(input("how many elements you enter: "))
list = []
for i in range(1,n+1):
    list.append(int(input("")))
pair = dict(zip(list,func(list)))
print(pair)
###############################

    
  
