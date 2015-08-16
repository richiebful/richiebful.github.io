---
layout: post
title: Starting with Shogi Programming
date: 2015-08-15 11:03:41
---

<p>Nothing like a summer project to stave off the doldrums, right? That's what I thought last summer. I was a young, overconfident programmer who thought they could tackle just about any challenge. Well, to say the least, I've thrown out an entire working framework once, made several abortive attempts at GUI with Qt and GTK+, and made minimal progress in the design of a game-playing AI.</p>

<p>But along the way, the lessons learned have been far more important. Tools for dealing with memory leakage <strong>valgrind</strong>, processing time <strong>gprof</strong>, documentation <strong>doxygen</strong> and debugging <strong>gdb</strong> have helped build maturity and discipline as a software engineer, rather than just a hacker. More than just copypasting and hacking together bits of code, I learned how to develop reusable, modular code. At the end of it all, one year later, my little command-line Shogi interface works.</p>

<p> <strong>Next steps: (listed by priority)</strong></p>
<ul>
 <li> GUI interface (GTK or QT?)</li>
 <li> Development of a Shogi AI</li>
 <li> Making online server for Shogi games</li>
 <li> Interface server with client</li>
</ul>

<p><strong>Interested in the project?</strong><br>
Have a look on <a href="https://github.com/richiebful/shogi">GitHub</a> <br>
Or get a copy of the most recent version: <a href="https://github.com/richiebful/shogi/archive/v1.0-alpha.tar.gz">source code</a><br>
<em>We only support POSIX-based systems at the moment</em>