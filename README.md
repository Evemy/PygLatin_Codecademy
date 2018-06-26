# PygLatin_Codecademy
Pig Latin creator from Codecademy. Saved for refernce.

echo "# PygLatin_Codecademy" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/Evemy/PygLatin_Codecademy.git
git push -u origin master

#included at the ending
pyg = 'ay'
#the word entered by the user
original = raw_input('Enter a word:')

#making sure the word entry is longer than 0 characters and contains no numbers
if len(original) > 0 and original.isalpha():
  #word contains the lower case version of the original input word
  word = original.lower()
  #first takes the first character from the word
  first = word[0]
  #new_word takes the word, adds the first character onto the end, plus the "ay" so: python =pythonpay 
  new_word = word + first + pyg
  #new_word copys the second character onward, removing the first character from the word so: python = ythonpay
  new_word = new_word[1:len(new_word)]
  #prints the new_word
  print new_word
else:
    print 'empty'
