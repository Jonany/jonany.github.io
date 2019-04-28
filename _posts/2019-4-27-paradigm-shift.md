---
layout: post
title: Paradigm Shift
---

## Paradigm Shift: My Journey to Functional Programming

#### Background

In the late Spring/early Summer of 2018, I set out to merge two intranet pages used for data maintenance into one incredibly functional, easy-to-use, time-saving masterpiece. Four months, a lot of PL/SQL, and two thousand lines of JavaScript later, I had a decently functional, relatively easy-to-use, time-saving mess :worried:. Don't get me wrong, the page works but trying to modify the functionality is a little like playing *Whack-A-Mole*. Make a change in one place and a bug pops up in another. Fix that bug and :rage: &mdash; well, you get the idea.

I needed to be confident that when I changed one part of my code I didn't unknowingly mess up another part. Enter _Unit Testing_ :tada:.

#### Unit Testing

I was already familiar with unit testing (although I knew it as regression testing) from my work in PL/SQL and I had seen how useful it was in that context. Since we had no equivalent infrastructure for other languages, I decided to find one. After a lot of research, some trial and error, and a few conversations with my supervisor, it seemed that [Jasmine][7] was the best option for our environment. As I began testing (:smirk:) that framework, I quickly realized that my code was not testable. Enter _Functional Programming_ (FP) :tada:.

#### Functional programming

There is [plenty][1] [of][2] [great][3] [content][4] [on FP][5] [in JavaScript][6] and I won't attempt to duplicate that content here.  However, to make sure we're on the same page here's my 10 cent explanation: FP seeks to minimize *side-effects* (changes in state) by enforcing *immutable data* (unchangeable once created) and *pure functions* (side-effect free). For me, FP had one big draw &mdash; the reduction in side-effects meant an increase in testability. All I needed to worry about was what to pass into the function and what I expected as a result.

#### Lessons learned

1. Unit testing is _well_ worth my time. Even though I'm not excited about writing tests first &mdash; I want to write code not tests! :unamused: &mdash; the benefits are definitely worth it. Writing tests helps me think through the functionality I'm creating and how it should work. Having tests to back me up when I change my code is pretty nice too.
2. Functional Programming is great! :grinning: It took some getting used to &mdash; my brain is still wrapping itself around currying :dizzy_face:&mdash; but it's been worth it. I like the methodical and systematic nature of FP. It helps me look at problems from a different angle and often come up with better solutions.

[1]: https://mostly-adequate.gitbooks.io/mostly-adequate-guide/
[2]: https://bethallchurch.github.io/JavaScript-and-Functional-Programming/
[3]: https://medium.com/javascript-scene/a-functional-programmers-introduction-to-javascript-composing-software-d670d14ede30
[4]: https://www.sitepoint.com/testing-functional-javascript/
[5]: https://youtu.be/Pg3UeB-5FdA
[6]: https://youtu.be/e-5obm1G_FY
[7]: https://jasmine.github.io/
