# Ruby

Official: https://docs.ruby-lang.org/en/3.2/index.html

Unofficial: https://rubyapi.org/ 

Unofficial: https://www.rubydoc.info/stdlib/core/index

Gems: https://guides.rubygems.org/rubygems-basics/

## Whitespace
Multiple sources from the Ruby course I'm on tell me to use tab as 2 spaces. Not as tabs, not as 4 or 6 or 8 spaces. Which had me wondering why. I tend to favor 4 spaces up to this point because I've found it the easiest to identify indentations without excessive white space. Is white space significant in Ruby like it is in Python? (I haven't read any Ruby beyond hello world at this point.) But from the 4 sources (just different sites with conversations), it's just convention for consistency and possibly to allow readable deeper nesting. I was directed to the unofficial guide at [caliban.org](https://caliban.org/ruby/rubyguide.shtml#indentation).

## Snake Case
I don't recall learning snake case before now. It is certainly more readable, particularly when involving acronyms. Camel casing and pascal casing with acronymns is a nightmare. I've worked around them by (a) avaoiding them, then (b) using underscores around them. But that's inconsistent. Perhaps I'll favor snake case outside of Ruby too.

## Rounding
Converting from float to int doesn't round. Which naturally led me to wonder about existing methods for floats since I currently can't imagine a scenario where I just want to chop off the decimal places. I found *.round*, which then led to reading the documentation on *.round* and playing around (*heh*) with the method parameters. Finally chaining together methods as such *2.5.round.to_i*. Overall, I am greatful that irb exists for me to play with that so early on. I find the learning curve of creating and running a file (no matter how minor that curve is) to be a barrier to this kind of silly experimentaiton during very early learning.

## Boolean
Most of my career has been spent on Salesforce. To see bools including nil as a "value" is plesantly surprising. Salesforce requires a value in their bools so they're *always* true or false and that's something I have to consider during the building of flows, formulas, and any other logic. I don't think I can really articulate why it's nice to have nil.

## Modulo vs Remainder
I'm glad I find math interesting instead of tedious. It has been a long time since I was in a classroom learning, mostly in passing, what a mod is. More-or-less my memory has it as "modulus is just the remainder." But it's not. I'm sure I knew that from high school math. But it's so long ago that the level of certainty I have is low. And now I'm in a small rabbit hole learning about it. I'm starting at [the big machine dot io](https://bigmachine.io/career/mod-and-remainder-are-not-the-same)  and a personal favorite [khan academy](https://en.khanacademy.org/computing/computer-science/cryptography/modarithmetic/a/what-is-modular-arithmetic) but I expect later today I'll be munching on popcorn while watching an hour long youtube video.

## Semicolon
It has been clear since I started looking at Ruby that semicolons weren't a thing. The Odin Project (input/output lesson) just explicitly stated they're not necessary but that you *could* use them. Semicolons allow you to run multiple commands in one line. This is new to me and fun to learn. And this brings me back to school when we talked about the ternary operators. They have a time and place. You can use it, but should you? Clarity should always be a top priority. Your code can be elegant and perfect and amazing, but if it can't be understood by future you AND others after you, what is the point? How can your code be maintained or used in the future? What are you communicating? Improper use of minimized code is like using a thesaurus to look smarter in an essay.You've obfuscated your message because communicating the message was not the goal. Be clear to the people you're talking to. Know your audiance. Assume future you is a little bit less knowledgeable than current you.

## Spaceship Operator
Not much to say here other than it's cute. How many languages have this? Have I seen it before? Is my memory of it just bad? 

https://en.wikipedia.org/wiki/Three-way_comparison Okay okay okay, I know strcmp in C isn't new to me. I'm going with my memory is just bad or no one told me it was also called a spaceship operator. I don't think I would have forgotten that name. 

## And v &&, Or v ||
Something about the word precedence isn't clicking for me. So now I'm ready perl documentation like reading this single word will suddenly make it click for me. It's like I'm learning *they're their there* again but just staring at the words out of all context. So this bit is just me working it out.

|| is like a division in a math equation
or is like a subtraction in a math equation
where = is an assignment with priority (precedence?) between || and or

So this is just BEDMAS for programming.

[This](https://press.rebus.community/programmingfundamentals/chapter/order-of-operations/) confirms that. Okay, so I am kind of understanding.

I'm not sure if staring at more examples helped me or if this site just had the right examples, but the women on rails post [here](https://womanonrails.com/operator-precedence-ruby) helped a lot. I still feel like I'm in a math class learning *they're their there* without examples (wrong class for the subject, clearly), probably because I'm not doing it. I should add doing something oddly complex just for the sake of getting precedence down.

## irb
### Options
As a part of The Odin Project I was reading the [this stackoverflow question about loading a file into IRB](https://stackoverflow.com/questions/13112245/ruby-how-to-load-a-file-into-interactive-ruby-console-irb/38533339) which had answers including options that I wasn't fully understanding. It took a little searching to find [die.net's page on Ruby options](https://linux.die.net/man/1/ruby) that included the -I and -r. This is one of those reading-it-doesn't-cement-it areas. Once I use the options more, and then come back to read this, I'm sure it'll click more fully.

### Completing Methods
While following along the lesson on [Data Types](https://www.theodinproject.com/lessons/ruby-basic-data-types) I saw irb display a little picklist/drop down. Took a little playing around to learn that tab will move me down the list of options. It also provided me clear instructions for viewing documentation on the method (alt + d). When ramping on a language and most of the information is more-or-less 1-1 with what you know, little things like this are fun to explore. The only issue I had was exiting the documentation view. ESC? nope. Ctrl + C? nope. Enter? nope. Typing out exit? nope. *Just the letter q.* I went a little squirrely for about two minutes trying to figure that one out.

## The Odin Project: Ruby Course
https://www.theodinproject.com/paths/full-stack-ruby-on-rails/courses/ruby

## Introduction to Programming with Ruby by Launch School
https://launchschool.com/books/ruby

The introduction of this book is part of the reading from The Odin Project. If I want to reitterate what I'm learning through The Odin Project, this appears to be a good source. They have other books covering topics like SQL, Agile, and Regular Expressions. I'll add these books to my ever-growing future projects list.

The Preparations chapter is also part of the reading from The Odin Project. The [Using the Command Line and irb](https://launchschool.com/books/ruby/read/preparations#usingcommandlineandirb) section includes troubleshooting for AWS Cloud9. Specifically fixing an issue for configuration (IRB.conf[:USE_MULTILINE] = false).

## Ruby Monday Study Group curriculum for beginners
https://ruby-for-beginners.rubymonstas.org/index.html

The tools of this curriculum is part of the reading from The Odin Project. It's another avenue for reitteration. They also have a testing for beginners path, which I'll be adding to my, again, ever-growing future projects list.

The most interesting part of the tools section for me was IRB. It gave me a simple try-something-new joy, which is important for me to keep the learning momentum going.
