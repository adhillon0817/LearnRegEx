# LearningRegEx: Matching an Email

During this tutorial, you will get to learn about the expression of matching an email. I will be giving a thorough breakdown of each part so that you can gain a stronger understanding of this expression. 

## Summary
This specific regex expression serves the purpose of validating a specific email address. Depending on the complexity of the expression, one may find a certain email address to be either valid or invalid based on the complexity of the regex expression. 
The following is a regex expression on matching an email:
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [Author](#author)


## Regex Components

### Anchors
Anchors are meant to catch a specific part of the text. Some anchors catch the front of the text and another anchor can catch the ending of the text. In the email regex, the main anchors used are ^ and $. The caret has the duty of catching the beginning the of the text area while the dollar has the duty of catching when the text has ended. Using one of each at the beginning and end of the text might not be sufficeient in some cases, so the user can insert an 'm' to catch the beginning of each line. 

### Quantifiers
The quantifiers of a regex expression are the '+' and '{2,6}'. The '+' will continue to tell the expression to match continuosly until it cannot match anymore. The {2,6} function also plays a similar role in attempting to catch as many times as withing 2 and 6 with the characters.

### Grouping Constructs
'()' are the grouping contructs in this specific function. This is where the multiple parts are set together in order to match the substring. In the email expression it looks like: ([a-z0-9_\.-]+) this is in one set of '()', then there is ([\da-z\.-]+), and ([a-z\.]{2,6}). These three parts are specifically set within the '()'.

### Bracket Expressions
Bracket expressions are surrounded by brackets! In the email regex there are three parts with '[]' being used around them: [a-z0-9_\.-] , [\da-z\.-] , and [a-z\.]. These brackets group together the parts of the text we are looking for. In the first bracket set, the expression is trying to match characters, lowercase, a-z. Also in the same first bracket set you can see that '\.' which is looking for all the periods ('.'). The other two [] functions play similar roles, based on what is in the brackets.

### Character Classes
Character classes are meant to match single character collowed by the \d. This is kind of like the (ctrl-f) function of searching through text for the specific characters you are looking for. In this function [\da-z\.-] meaning it willl look for the characters in the specific given range of a-z.

## Author
A student at UW Coding Bootcamp:
Avleen Kaur Dhillon