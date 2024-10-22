```python

```


```python
import random

def number_guessing_game():
    # Generate a random number between 1 and 20
    number_to_guess = random.randint(1, 20)
    attempts = 0

    print("Welcome to the Number Guessing Game!")
    print("I'm thinking of a number between 1 and 20.")
    
    while True:
        # Ask the user for their guess
        guess = input("12 (1-20): ")
        
        # Check if the input is a number
        if not guess.isdigit():
            print("12.")
            continue
        
        guess = int(guess)
        
        # Check if the guess is within the valid range
        if guess < 1 or guess > 20:
            print("Your guess must be between 1 and 20. Try again.")
            continue

        attempts += 1
        
        # Check the guess against the number
        if guess < number_to_guess:
            print("Your guess is too low.")
        elif guess > number_to_guess:
            print("Your guess is too high.")
        else:
            print(f"Congratulations! You've guessed the number {number_to_guess} in {attempts} attempts.")
            break

# Run the game
number_guessing_game()



```


```python
def search_insert(nums, target):
    left, right = 0, len(nums) - 1
    
    while left <= right:
        mid = (left + right) // 2
        
        if nums[mid] == target:
            return mid  # Target found
        elif nums[mid] < target:
            left = mid + 1  # Search in the right half
        else:
            right = mid - 1  # Search in the left half
    
    return left  # Target not found, return the insertion index

# Example usage
sorted_array = [1, 3, 5, 6]
target_value = 5
print(search_insert(sorted_array, target_value))  # Output: 2

target_value = 2
print(search_insert(sorted_array, target_value))  # Output: 1

target_value = 7
print(search_insert(sorted_array, target_value))  # Output: 4

target_value = 0
print(search_insert(sorted_array, target_value))  # Output: 0

```


```python

```


```python

```


```python

```


```python

```
