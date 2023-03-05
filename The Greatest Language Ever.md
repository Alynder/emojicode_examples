# The Greatest Language Ever

### How to make a cure program with emojicode

In this article I'll be covering the greatest coding languge to learn how to make anything! It's called Emojicode. This is an open-source programming language that uses emoji characters to represent its syntax, created in 2014 by Theo Belaire.  When working in Emojicode, emojis are used to create variables, functions, and control structures. Since this is a statically typed language variable types need to be declared before use, but it also supports object-oriented concepts like classes and inheritance. This language can be run on every OS as of right now, and is a super fun way to code especailly if you're a non-native english speaker. This is great because pictographic repsrestations can bring us all together and allow us to speak the same language in a way similar to math.

#### What tools I'm using for this article
In this walkthrough I'm using a debian based OS, so my tools may be different than what your OS may require. Below is my list of tools.

- [Geany](https://github.com/geany/geany) and opensource linux IDE
- A form of [IBus](https://en.wikipedia.org/wiki/Intelligent_Input_Bus), which allows you to pick the emojis and place them in your editor (this one is called emoji picker)
- Debian based linux
- g++ (but you can use any C++ compiler) 
- [Emojicode](https://github.com/emojicode/emojicode)

This article will look a little different because I'm using a linux OS, but you can always [read the docs](https://www.emojicode.org/docs/) on how to use it on your preffered OS.

#### Getting started with installation
There are a couple ways to install Emojicode on your computer, but they have a cool [magic install page](https://www.emojicode.org/docs/guides/) that can tell you exactly what to do.
My install commands are below.

```sh
wget https://github.com/emojicode/emojicode/releases/download/v1.0-beta.2/Emojicode-1.0-beta.2-Linux-x86_64.tar.gz -O emojicode.tar.gz \
&& tar -xzf emojicode.tar.gz && rm emojicode.tar.gz \
&& cd Emojicode-1.0-beta.2-Linux-x86_64 && ./install.sh \
&& cd .. && rm -r Emojicode-1.0-beta.2-Linux-x86_64
```
This is the output of that command.
<<< PICTURE HERE>>>>


Now that we have everything installed, lets move on to some code!


#### How does this whole thing work?
I want to write some code so now what?
To start, all Emojicode file extention end in filename.🍇 but since we can't do that in our average file same it translates to filename.emojic.
Next up let me go through some points to speed this along.

- Put 🏁  in the beginning of a line to indicate what blocks of code will be executed
- To start a block of code use 🍇
- To end a block of code use 🍉
- Want to print something just use 😀 🔤 Words to print 🔤 ❗

These are some of the basics, but there's way more to it so lets go through some examples!

#### Printing some things
So first up we'll be printing a nice haiku for fun!
I'll even add a single comment in this example.


🏁🍇
💭 This is a single line comment for fun
😀 🔤Emojicode is great,🔤 ❗
😀 🔤Fun and expressive code,🔤 ❗
😀 🔤no sadness, just joy.🔤 ❗  
🍉

Now we need to save our code, and run it through our compiler to make a nice executable file. Following the steps below.

```sh
$ emojicodec haiku.emojic 
$ ls
 haiku  haiku.emojic  haiku.o  
```
As you can see we compiled the code and it generated two files, we'll need just the executable `haiku` file. See the output below.

```sh
$ ./haiku 
Emojicode is great,
Fun and expressive code,
no sadness, just joy.
```

#### Silly math tricks and vaiable manipulation
Next up we're going to do a couple of things at once, a little bit of math and the changing of the variable.

Starting with assigning our variable to 0

0 ➡️ 🖍🆕x

We're creating this new variable by using the crayon emoji and the new emoji next to our vairable name. While also assigning that variable to 0.

Next we'll print a line that includes our variable using the magnets emoji.

😀 🔤The value is 🧲x🧲 🔤 ❗

Next we'll change the variable using the Plus sign and arrow emojis.

x ⬅️➕ 1

Then print another line with the value. I'll continue this for a while, and print the final value.
Here's what I did below.

🏁 🍇

💭Updating a variable using math 

0 ➡️ 🖍🆕x

😀 🔤The value is 🧲x🧲 🔤 ❗

x ⬅️➕ 1

😀 🔤The value is 🧲x🧲 🔤 ❗

x ⬅️➕ 15

😀 🔤The value is 🧲x🧲 🔤 ❗

x ⬅️➖ 9

😀 🔤The value is 🧲x🧲 🔤 ❗

x ⬅️➗ 2

😀 🔤The final value is 🧲x🧲 🔤 ❗
🍉

Next we'll compile this using our emojicodec, and then use our executable code too see the outcome.

```sh
$ emojicodec math.emojic 
$ ./math 
The value is 0 
The value is 1 
The value is 16 
The value is 7 
The final value is 3 
```
As you can see everything printed out as the variable was updated with the new math.





