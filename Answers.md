## 1. Review these translations

Here are 4 Objective-C translations of the same code:

- https://gist.github.com/anonymous/0b2175c5bc5c2bf4e272b0a78f999158
- https://gist.github.com/AhmetAbak/550647df95298863dbb39b7bb978b7f6
- https://gist.github.com/vian/bf238a869764c79e818db4b8d8521265
- https://gist.github.com/ezavalko/cf85ee5a55b182c0288b2ec8aab35909

We’re looking for Objective-C that is conventional, clear, clean, idiomatic, and follows Objective-C best practices.

In your reviews, tell us some things you’d correct about the code in a code review. What’s good about the code? What’s bad about it? Include specific technical examples. Your reviews do not have to be long.

Also, assign each translation a score from 1-4:

1: excellent code. This programmer is clearly an Objective-C expert. We should hire them.  
2: good code. This programmer is good at Objective-C but will need some guidance. We could hire them if we needed to.  
3: ok code. This programmer can write Objective-C but has a lot to learn. We should not hire them.  
4: unacceptable code. This programmer does not know Objective-C. We should not hire them.  

Finally, rank the gists from best to worst.

==============================================================================
###### In 3th file, declaration of function is wrong.
-- Original code
	NSInteger ALGHighestProductOf3FromIntArray(NSArray *arrayOfInts) {

-- Updated code
	 + (NSInteger) ALGHighestProductOf3FromIntArray: (NSArray *) arrayOfInts {

4th file has issue as following code.
**Original code**
     for (int i = 0; i < arrayOfInts.count; i++){
        NSNumber * number = [arrayOfInts objectAtIndex:0];

**Updated code**
     for (int i = 2; i < arrayOfInts.count; i++){
       NSNumber * number = [arrayOfInts objectAtIndex:i];

2nd developer has clear knowledge about obj-c.
4th developer has issues in the source code.
1th developer knows obj-c, but he is not perfect.
3th developer doesn't know obj-c.

**Ranking**
* 3. https://gist.github.com/anonymous/0b2175c5bc5c2bf4e272b0a78f999158
* 1. https://gist.github.com/AhmetAbak/550647df95298863dbb39b7bb978b7f6
* 4. https://gist.github.com/vian/bf238a869764c79e818db4b8d8521265
* 2. https://gist.github.com/ezavalko/cf85ee5a55b182c0288b2ec8aab35909


## 2. Read through this content:

- https://www.interviewcake.com/question/objectivec/stock-price?expand=1
- https://www.interviewcake.com/concept/objectivec/array
- https://www.interviewcake.com/concept/objectivec/garbage-collection

Look for:
 
- Cases where we need to change wording. Maybe we say “list” where we should say “array.” Maybe we say `IndexError` but it should be `ArrayIndexOutOfBoundsException`.
- Incorrect explanations. Maybe we’re wrong about your language having mutable strings, lazy evaluation, or garbage collection.
- Mistakes or inconsistencies in code.
 
For each page, explain the changes that should be made. Be specific and actionable with your changes, using explicit instructions. (Don't just say what's wrong.)
 
Identify any changes that would make our content better for our Objective-C users, but also, be careful not to be the type of reviewer who needs ducks (#5 here):
 
https://blog.codinghorror.com/new-programming-jargon/

==============================================================================




















## 3. When does your language use the words "function" and "method"?

Explain briefly and clearly.

==============================================================================

**Method**  depends on object but **Function** is not.


## 4. Answer these questions about strings

In our question about building a word cloud (https://techinterviewprep-stag-pr-1880.herokuapp.com/question/word-cloud?expand=1) we have these 2 paragraphs:

> We could build up our current word one character at a time and append its value to the list every time we hit a space. This works, but every time we append a character we'll be making a new copy of the word. If our input is one long word, then creating all these copies is O( n^2 ).

> A more efficient strategy is to keep track of the index where our current word starts and its length. When we hit a space, we'll copy the characters out of the input string into a new word and append it to the list. That way our splitWords function is O(n).

Questions:

1. Is the first paragraph accurate? Would building up a string one character at a time be O(n^2) in your language? Or does your language have an O(1) append-character-to-string operation?
1. Does your language have a particular word/phrase for "string slicing" – how we grab the subset of the string. Is it "string slicing" or something else?

==============================================================================





## 5. Are there things you'd change about our style guide?

https://gist.github.com/kaplanoah/71446132717d9c83350e06dad91a2981

Give one or two examples, if you have any, and explain them briefly.

==============================================================================




## 6. Do you know big O notation?

You should know big O notation well enough to understand the examples here:

https://www.interviewcake.com/big-o-notation-time-and-space-complexity

==============================================================================





