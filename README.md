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

### Inspirational talks and lectures

[Bret Victor - Bret Victor - Inventing on Principle](https://www.youtube.com/watch?v=PUv66718DII)

[The Mother of All Demos, presented by Douglas Engelbart (1968)](https://www.youtube.com/watch?v=yJDv-zdhzMY)

### The rule of 10

The rule of 10 states that for every factor of 10 in scale, a new set of problems dominates.

The idea here is that software design is not scale invariant. Significant scale differences change things in fundamental ways (eg. human-scale insects wouldn't work and viceversa). As a counterpoint to that, the ideas about abstraction and process _are_ scale invariant, so eg. the concept of a loop (so, repetition) is so fundamental to the idea of automation that it appears  in one form or another at every level of abstraction.

### The confession of an idiot programmer [1](https://wiki.c2.com/?IdiotProgrammer)

> I am an idiot. That has profoundly affected the way I code. Everything must be simple enough for a child to understand, and even then, I struggle.
>
> Being an idiot has forced me to refactor mercilessly. If I don't, there's no chance of my understanding my code. And if I don't understand my code, there's no chance of my getting it to work.
>
> I've seen people who can solve complex problems, and I admire them. Alas, I'm not one of them. So whenever I have to solve a complex problem, I make it simple first.
>
> If I can't make a problem simple, it's usually because someone else insists that it remain complex. In that case, I have to wait for someone smart to fix it (thank you, smart person), or for someone to change their mind and allow me to make the problem simple.

I can relate a lot to that. I never considered myself a particularly fast coder or snappy thinker. I know people who are a lot faster than me. My "secret" is that I simply stay with problems longer. When you stay with a problem longer, its complexity peels away layer by layer until the problem becomes so simple that you can even tell it to your stupid computer that takes everything literally.

At my last teaching gig I used to tell students that if you can formulate your problem precisely, the code basically writes itself. People's first reaction when they hear this is something like "if only that were true, programming would be so simple". But then they are surprised to find out how difficult it is to actually formulate an idea with any amount of precision. How many assumptions are implied and must be made explicit, how many are wrong and must be discarded. 

This process can be anxiety-inducing for someone who's not used to it because it makes you acutely aware of the gap between your mental moddel of the world and the reality of it. But this is precisely what enables you to progress and narrow that gap. Thinking is transitioning between multiple states of failure with the hope that it will all end in a state of success. 

Richard Feynman said that if you can't explain it to your grandmother, you don't understand it well enough. If your grandmother can understand it, this demonstrates that the little branch from your internal knowledge tree in your head that you were trying to transfer to her mind is self-contained enough that she can integrate it in her own knowledge tree making all the necessary connections. If this fails, your idea contains assumptions (i.e. context) that you're not aware of and that you must discover.

Discovering that you're an idiot programmer is humbling and liberating. You don't have to prove anything to anyone which makes you more relaxed, and getting more aware of your limitations is always a good thing because it allows you to optimize for them instead of fighting to overcome them.
