<h1>Welcome to the Love Calculator!</h1>

<p>To receive input of two names:</p>

<pre>
name1 = input("What is your name? \n")
name2 = input("What is their name? \n")
</pre>

<p>To convert all the input to lower case:</p>

<pre>
name1 = name1.lower()
name2 = name2.lower()
</pre>

<p>To calculate the love number we have to combine the two name and count the occurence of true love in it:</p>

<pre>
combined_string = name1 + name2
combined_lowercase_string = combined_string.lower()
t = combined_lowercase_string.count('t')
r = combined_lowercase_string.count('r')
u = combined_lowercase_string.count('u')
e = combined_lowercase_string.count('e')

true_count = t + r + u + e

l = combined_lowercase_string.count('l')
o = combined_lowercase_string.count('o')
v = combined_lowercase_string.count('v')
e = combined_lowercase_string.count('e')

love_count = l + o + v + e

true_love_count = str(true_count) + str(love_count)

print(f'the love count for {name1} and {name2} is {true_love_count}')
</pre>

<p>The conditional statement to generate message depending on the number gotten:</p>

<pre>
if true_love_count <= '40' and true_love_count == '50':
    print(f'your love score is {true_love_count}, you may not be the best for each other')
elif true_love_count > '50' and true_love_count < '90':
    print(f'your love score is {true_love_count}, you go together like coke and menthos')
else:
    print(f'your love score is {true_love_count}, you are good together')
</pre>
