# Beginning C\# for BAMFs #

## Hello Severed Head

You got this severed head just like me...pretty rad, right? It’s the smartest severed head around. At least it said so on the box. Strangest thing though, it doesn’t have a mouth, or eyes, or ears, or a nose.

...and wouldn’t you know it, you just found a flyer for a *smartest severed head* contest. The winner gets free bacon for life. The thick kind. 

Have you ever worried that you might not have a good way of proving that your severed head is the best when there's bacon on the line? Then you’ve come to the right place. 

### Visual Studio

Your first task is to install Visual Studio on your computer. Visual Studio is the app we use to facilitate communication with disembodied heads for the purpose of teaching them to do things for us, so they can work while we sit and watch cartoons. 

Usually there would be painstakingly detailed instructions in this section detailing how to set up your development environment. In my experience - by the time everything is written and published all of the pictures would look different and the instructions would be wrong because things change over time. It would probably cost you tiome and confusion. Instead of doing that, I’m going to be lazy and I’m not going to bother writing any of that. Better for you to look to the official website.

To get started do the following:
- Install Visual Studio - https://visualstudio.microsoft.com/
	- **Important** - When it asks you which *workloads* to install ensure that you select “.Net Desktop Development”, or you won’t have the template to make a console application. 
- Make a folder on your drive to put all of your projects.
	- I’d recommend that you name it something flashy and clever like “projects” and maybe put it in your user directory: mkdir ~/projects
- Create a new solution (file -> new solution)
- Make the template a new console application
- Create it in the directory you created for your projects
- Name the project/solution hello_world
- If it asks for a version, the .NET version and Visual Studio versions don’t really matter for the stuff in this book. I’m going to show you things that are fairly universal so you can just pick the version with the biggest first number.
- Once the solution is created, locate the solution explorer and poke around a bit. It basically gives you a listing of all the files in your project and you can click them to look at them in a text editor. 
- Locate a file in the Solution Explorer called Program.cs and open it up in the editor

If you got this far - congratulations. You’ve got what it takes to be a novice severed head trainer and I officially confer upon you this title. Your parents will be so proud. 

### How to How To

We’re going to start looking at code shortly and I want to give you some advice for getting the most out of it.

*First*, don’t stress out too much about understanding each and every little thing. For the time being just follow along and TYPE IT ALL IN BY HAND. 

*Second*, If you don’t understand something just accept it as magic and move on. 

The end goal of this book is that you should be familiar enough with object-oriented programming that you can branch out where you like at the end and learn the rest through context, repeated usage and documentation.

When I was a software pup I had to read my basic books several times over before everything made sense. I have read many of these sorts of books over the years and I found a practice pattern for learning stuff like this that seems to work really well for me. Give it a try if you like:

1. Read the book once straight through and type all of the examples in. 
	1. Get the programs working whether or not you understand everything in them. It’ll get all the words and ideas bubbling around in your brain-bucket.
1. Read it again but much faster. Just lightly skim over the parts you understand. It’s the parts you don’t understand where you need to spend the lion’s share of your time.
1. Repeat until you understand all of it. Then figure out where to go next.
1. Experiment. Try stuff out. Don’t be a clingy stalker and creep on my book and refuse to do anything else. Try to make your own stuff to learn how to express yourself.
1. Do not be afraid to use other sources to help fill in the blanks.

### WTF IS A Programming Language

Alright, so let’s stop flapping gums and get to it then. That file I had you open in your editor; *Program.cs*; should look something like this:

```
using System;

namespace hello_world
{
	class Program
	{
		static void Main(string[] args)
		{
			Console.WriteLine("Hello World!");
		}
	}
}
```

This stuff you see typed in here is the programming language code and this language is named C# (pronounced See Sharp). 

One of the ways that humans communicate is by utilizing meat vibrations. Humans push air through various configurations of meat in order to produce sounds that they associate with concepts. The individuals involved in said communication must agree upon which sounds correspond to which concepts, or they will not be able to comprehend one another. We call this process *talking*. 

We then abstract this whole talking idea down further into drawings that we use to represent specific sounds. We smash these drawings together to form a map that represents the correct order of meat-configurations required to speak the labels to communicate the desired concepts. By doing this we gained the ability to archive sounds and give them to others without needing to speak or even be there. We call this process *writing*.

Unlike us, computers base very little upon the vibrations of meat. Our meat-based communication is very difficult to explain to anything that didn’t evolve to communicate using air and meat. 

Computers are more electrical in nature and lend themselves more to concepts like ON/OFF or 0/1 or true/false, than they do to concepts based around meat vibrations. For computers, everything has to be defined in terms of something else down to the point you are left with nothing but 1s and 0s. As you can imagine a human might have a *very* difficult time seeing a funny meme if you show them millions of 1s and 0s; but a computer has no issue at all with it. A computer translates those 1s and 0s into an image and then lights up the correct pixels on your monitor almost instantly. 

So how do we bridge this communication gap? How do we have a conversation with computers seeing as how we don’t share a natural communication medium that makes sense to the other? Computers can think like a head but they have no meat to talk and no ears to hear vibrations. The reverse is also true, you don’t understand electrical or binary stuff very well. I am assuming that you have very few ports. I don’t have that many.  

To explain how we solve this issue, have you ever watched those old Star Trek movies where they could talk to aliens who spoke crazy alien languages by using a translator? The translator made it so that everyone heard the conversation in their native language. Only the translator itself needed to understand both languages and then everyone could happily talk through it. 

The translator in this story is known as a *compiler* in programming. When you type instructions (code) and build your project what you are essentially doing is running your code through a translator that turns it into something a computer can understand. If the computer needs to talk back to give you error or info messages messages the compiler will also communicate that back to you. You can then run the executable file that is generated for the compiler and the computer will be able to follow the instructions you communicated in code.

The process that the compiler goes through to translate your code into executable instructions is called *compiling*.

### The Main Method

Now that we have some of the external concepts explained, let’s jump back into code. For now we don’t need to focus much on understanding most of the code we’ve seen. When I started out I thought it was very important to understand every single piece of text in the code. Don’t do that because chances are you are missing some required concepts and we are going to talk about when it makes more sense. For now the only part you need to concern yourself is where I put the rectangle below:

```c#
static void Main(string[] args)
{
	CODE GOES HERE
}
```

![Main Image](images/Hello%40Severed%40Head/hello_world.png)
