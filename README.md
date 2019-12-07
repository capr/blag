## Why does everybody have to be so stupid?

That's right. I'm a hater. Not a week passes before I ask myself this question again.

Programming has eaten my life. And it still does, because I love it so much.
But boy, if I were to count the man-hours we're losing every day in this 
activity, profession, whatever you like to call it, doing useless crap that 
we would never have to do if we'd only be just a little bit smarter on 
how we do it, the graveyard would be miles long.

I have accumulated a lot of negative thoughts about this industry over the years,
and I'm going to vent in here until something happens, either I get tired, 
indifferent, or realize my ignorance and change the way I see things 
(fat chance - not with that attitude, hater boy). Well, anything's possible. 

Until then, stay tuned, because I have a lot of things to get off my chest.

#### UPDATE Dec 2, 2019

Here's a shortlist of topics that I'd like to talk about:

### The way we distribute and run software is fundamentally broken

This is a big one and needs a lot of explaining. The software culture and industry is shaped and regulated by the ways in which software gets on people's computers. The biggest fights in the industry are about who controls the platforms that software runs on. It's why Apple made the iPhone and why Google made Android and Chrome. It's the reason why Microsoft dominates the desktop market and the reason why Linux doesn't (but could, if they would understand this).

TODO: Talk about operating systems, browsers, apps and app stores, docker, Linux distributions, etc., their implications, and how different models of software distribution could change the loci of control and shift the power towards users and smaller players.

### The Internet culture is shaped by a limitation of the IP protocol

The way the Interent works, it is hard to connect two random computers on it together. This asymmetry led to the client-server idea that is basically our culture on how the Internet works today. This gave rise to the web, a revival of terminal/mainframe model of the 70s (now called "cloud computing" and "web apps"), exacerbating the separation between technology producer and technology consumer. But if it weren’t for this basic limitation in the IP protocol, the Internet and the way we use it to communicate and the kinds of apps that we would envision for it might look very different today.

### Most programming is at the wrong level of abstraction

This is a complex topic, but it boils down to how we view programming languages in this culture. Even though there's a proliferation of new languages in the last years, every one of them tries hard to create its own bubble, to distinguish itself and specialize without also focusing on interoperability and embeddability so that it can be easily used from other languages and contexts. Moreso, we simply aren't yet able to envison a tool that can work well at multiple levels of abstraction, which leaves us endlessly reinventing the same wheels with every new tool, eg. every language reimplements the same cross-platform GUI library.

### C in recent years

This is targeted at C compiler writers, which these days means GCC and LLVM people. Compiler writers serving the standards people instead of serving their actual users. Standards people don't understand their users because most of them don't have any experience producing actual shippable software. The spherical cow in a vacuum that is the C abstract machine combined with the ever-growing plague of undefined behavior has made this language close to unusable in recent years. It wouldn't matter if C would die, but this beast is hard to kill, the core language being too good for its own sake even though everything around it (the preprocessor, the tools, the endless build systems) sucks.

#### Update Dec 3, 2019

### Text-based protocols

If you ever get to read the RFCs on the HTTP protocol, that marvelous piece of engineering that even got its inventor the blessings of Her Majesty The Queen herself, you'll quickly realize what a miracle it is that our computers even start when we plug them in. I for one am amazed how Google can track my online behavior so well based on those cookie RFCs because if my calculations are correct, those things should just not work. So there you go. Something to be grateful for. You're welcome.

#### Update Dec 7, 2019

### Design patterns and object-oriented programming

Let's see what some reputable people in the field have to say about it:

"Design patterns are spoonfeed material for brainless programmers incapable of independent thought, who will be resolved to producing code as mediocre as the design patterns they use to create it." - Christer Ericson, tech lead at Sony.

"Object-oriented programming is an exceptionally bad idea which could only have originated in California." - Edsger Dijkstra.

"The problem with object-oriented languages is they’ve got all this implicit environment that they carry around with them. You wanted a banana but what you got was a gorilla holding the banana and the entire jungle." - Joe Armstrong, Erlang creator.

This reminds me to hate a little on Martin Fowler some day... that scarf-wearing hipster, the Tony Robinson of web programmers that lures people with 50 dollar terms like "dependency injection" and "mob programming" but I can't seem to find any evidence that he's ever written a single line of code in his life.
