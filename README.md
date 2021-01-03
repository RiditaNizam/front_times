# front_times
CodingBat Python Warmup-2

Given a string and a non-negative int n, we'll say that the front of the string is the first 3 chars, or whatever is there if the string is less than length 3. Return n copies of the front.

def front_times(str, n):
  
  answerString = ""
  
  for i in range(n):
    if len(str) == 1:
      answerString += str[0]
    elif len(str) == 2:
      answerString += str[0:2]
    elif len(str) >= 3:
      answerString += str[0:3]
  return answerString
