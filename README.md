# list-comprehension

### Each lab should be a function in a single Python file

#### Lab 1: Grade Calculator
**Objective**: Write a program that calculates the letter grade based on a list of scores.
Instructions:
- Ask the user to input multiple test scores (store them in a list).
- Calculate the average score.
- Use conditionals to assign a letter grade based on the average:
A: 90-100
B: 80-89
C: 70-79
D: 60-69
F: below 60
- Print the average score and corresponding letter grade.
scores =[]

while True:
  score_imput = input("Enter a test score (or type 'done' to finish): ")

  if score_input.lower() == 'done':
    break
  try:
    score = floar(score_input)
    scores.append(score)
  except ValueError:
    print("Invalid input. Please enter a valid number.")

if len(scores) == 0:
  print("no scores were entered.")
else:
  average_score = sum(scores) / len(scores)

  if average_score >= 90:
    grade = 'A'
  elif average_score >= 80:
    grade = 'B'
  elif average_score >= 70:
    grade = 'C'
  elif average_score >= 60:
    grade = 'D'
  else:
    grade = 'F'

print(f"The average score is: {average_score;.2f}")
print(f"the letter grade is: {grade}")


#### Lab 2: Even and Odd Numbers Counter
**Objective**: Write a program that counts the number of even and odd numbers in a list.
Instructions:
- Ask the user to enter multiple integers separated by spaces, and store them in a list.
- Use a loop to iterate through each number in the list.
- Use conditionals to determine if a number is even or odd and keep a count of each.
- Print the counts of even and odd numbers.

#### Lab 3: Unique List Merger
**Objective**: Create a program that merges two lists and removes duplicate items.
Instructions:
- Ask the user to enter two lists of numbers, each separated by spaces.
  For example: `1,2,4,6 2,5,7,1`
- Convert each list of numbers to integers and combine them into one list.
- Use a loop and conditionals to remove duplicate entries.
- Print the merged list without duplicates.
- Allow the user to repeat the process with different lists or type "exit" to quit. Make sure to use the keyword `break` in your implementation.
