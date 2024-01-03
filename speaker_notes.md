# speaker notes

Hi! Welcome to my presentation about how to contribute to the Rust project. There are numerous ways
to help Rust by contributing to it, and I'm going to list some of them, show you how to do it
and point you to further resources about it. So after my talk, you hopefully have the knowledge and
motivation to get started yourself if you're interested.

But first, who am I to talk about this? I'm nils, and I've been a member of the compiler contributors
team for over a year now. In addition to contributing code to the compiler I've also been involved in
other things, like helping other people contribute to the compiler, triaging issues and of course shitposting on Discord.

But this talk here isn't just mine alone, other people helped with this too, like these silly bingles.

So, let's start contributing to Rust. Maybe some of you here have contributed something to Rust before,
(maybe you didn't even think it was a contribution), and I assume some of you have wanted to do it but have
never done it for various reasons, like not knowing where to start or even thinking you're not good enough to do it.

Here's the good news for that: I'm going to tell you a lot of different ways to get started, no matter
your experience level. There are so many things to do that there's something for everyone.
Sure, there are some areas that require domain-specific expertise, like writing a MIR optimization in the
compiler requires good knowledge of MIR, but there are also things that don't even require knowledge of Rust,
so even if you're still a beginner you can help, and I can guarantee that you will learn a lot.

The only thing you really need is some spare time and interest. Some tasks are very time intensive, but
other tasks require a lot less time. That said, if you don't have any spare time, then it's going to be hard.

With that out of the way, let's look at some places you can contribute to.

First, we're going to look at ways to contribute that don't involve opening VSCode or whatever your favourite editor is.
When talking about contributing to open source projects, we usually think of contributing code, like opening Pull Requests.
While this is an important part of any open source projects and no less true in Rust, it's also by far not the only thing to do.
And especially those other tasks are often forgotten and underappreciated. We're also not great at this, there's a very nice page
called `thanks.rust-lang.org` that contains a list of contributors, but it only counts commit and review counts.

The first thing I'm going to talk about is triaging issues, something that I have also done a lot myself.
Triaging issues is great because it's easy to get started and you can put in very variable amounts of time.
You can triage one issue in two minutes, or you can spend 2 hours on an issue. It always depends on the
issue and how much time you want to put in, even the small work is nice.

Some of the things that are involved when triaging issues are labelling, minimization, bisection and adding tests.

Labelling is the task here that takes the least time. We have an example issue here, that requests that the standard
library documents the memory ordering guarantees for the thread spawn function.
Let's think about what this is: This is a *feature request* for *documentation* about *threads* and *atomics*.
The feature request is to the *library API team*, as it's about a guarantee.

So we add those labels. Remove needs-triage, as we're doing triage, add the docs, thread and atomics area, the category
feature request and the team libs api. If you're not part of a team that has write access to the repository, you can leave
a comment with rustbot as shown here. If you're interested and want to know more, see the link below.