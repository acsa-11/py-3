# py-3
def is_prime(num):
    if num < 2:
        return False
    for i in range(2, int(num**0.5) + 1):
        if num % i == 0:
            return False
    return True

def print_composite_numbers(start, end):
    for number in range(start, end + 1):
        if not is_prime(number) and number > 1:
            print(number)
