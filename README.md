
Given a string, we'll say that the front is the first 3 chars of the string. If the string length is less than 3, the front is whatever is there. Return a new string which is 3 copies of the front.

front3('Java') → 'JavJavJav'
front3('Chocolate') → 'ChoChoCho'
front3('abc') → 'abcabcabc'


code:

def front3(str):
  if len(str)<=3 and len(str)>0:
    str = 3*str
    return str
  if str>3:
    str = str[0:3]
    str= 3*str
    return str
    
  return str
