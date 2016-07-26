# A primer on open source licensing

## A Disclaimer
I'm not a lawyer. I have no formal training in law, and this document is only for educational purposes. 
I make no assertions about it's correctness.

This document is largely my notes from reading the following book:
	
>Laurent, Andrew M. St. Understanding Open Source and Free Software Licensing. Accessed July 25, 2016. 
>[http://shop.oreilly.com/product/9780596005818.do](http://shop.oreilly.com/product/9780596005818.do).

This book is available for free under a Creative Commons NoDerivs license and you should read it if you are interested.
Technically, this may be a derivative work, but I'm asserting that a summary for educational purposes is fair use, 
especially since I've referenced my source.

# Some preliminary definitions

- **What is copyright?**

A concise definition goes like this: 

Copyright is the concept that the first person to express an idea in a tangible manner (e.g. a particular representation of a mathmatical algorithm in computer code), reserves the right to profit in a tangible way from that expression (making money from it). No one else can profit from that particular expression of the mathmatical algorithm without the originators permission.

The idea of copyright also precludes others from unauthorized creation of a 'derivative work',e.g. a larger piece of code which incorporates the originators copyrighted work. What consititudes a 'derivative work' is a large portion of the nuance associated with open software licensing.

>Contrary to popular belief, any work created today will **automatically** be copyrighted. No line reading "(C) Copyright My Name 2016" would be nessecary for this document to have copyright protection. However it is considered good practice to include some such to make it explicit.

- **Limitations on Copyright:**

- *Work for hire*  
If a person creates an expression of an idea in the context of being compensated by another to do so, then the copyright belongs to the employer, not the employee. 

>Most software created by programmers for pay is legally interpreted as falling under this exception, with the rights holders being their employer. Open source licensing was originally introduced to change this situation by denying an exclusive right to profit to anyone by making the materials nessecary to profit freely available

- *Fair Use*  
This is not an well defined exception, but the gist is that exceptions are made to copyright when the expression is used in certain uses which do not impact the orginator's exclusivity to profit from thier work. Includes things like reviewing and criticizing the work.

- *Transformative Derivative Works*  
This refers to changing the work so fundamentally that a new work is created and the copyright for the derivative work is then held by the person who 'transformed' the work. Again, where the line between a derivative work and a transformative derivative work lies is a major issue in software copyright.

# Why isn't traditional copyright good enough?

Software is in a unique position compared to say, music. While derivative works such as DJ mixes or 'mashups' do exist and in some cases can generate revenue for their creators, people usually are more interested in buying 'Free Bird' on iTunes than the techno remix. 

A computer program, on the other hand, is often most useful as a component of a larger project. For example, a matrix inversion algorithm implemented in a clever and fast way is just an academic curiousity until it's incorporated into a faster and more accurate weather prediction model. This makes the question of what constitutes a 'derivative work' both controversial and important.

Also, software, unlike an Eagles song, is not art (for a given value of 'art'), meaning that you don't have to be a member of the Eagles to add to the work. Software can be, and often is, made better for having multiple contributing authors. In the matrix inversion example, a feature of a clever implementation of an algorithm is often it's brevity. Although it took many hours of work to come up with the code, it may only take a few minutes for an uninvolved mathemetician to read it, and provide a constructive minor change or feature addition which would increase the value of the work.

# Open Source Principles

## Open Distribution

Traditional software copyright makes it illegal to copy or redisribute software for money or for free. This has proved a very difficult rule to enfore (nod knowingly if you've ever installed a burned CD copy of any Microsoft product...actually better not, they might be watching...)

Open source software is subject to varying degress (depending on the license) to the 'open distribution' priciple, meaning that you are allowed to copy and redistribute the software for pay or for free.

## Open Modification

Traditional software copyright precludes any creation whatsoever of derivative works. "Open modification" means that you are provided with both the means and the permission to modify and distribute modified versions of the software, for pay or for free.

## Generational Limitation

This simply means that others cannot claim to be the work's creator, and must acknowlege the creator's copyright. Most open source licences reserve this right. Some additionally require that any derivative works must also be licensed under the same license. This is called *copyleft*.

# Certified Open Source Licences:
	
>Open source licenses are certified by the Open Source Initiative. In order for a license to be OSI-Certified (which all commonly used liceses are) it must satisfy all of the following critera. I have paraphrased the following from the OSI formal legal text.

1.  No prevention of anyone from selling or giving away the licensed software as part of a package of software, (to clarify this is __non-exclusive__, i.e. everyone who has a copy has an equal right to sell it or give it away, regardless if they are the author or not)
2.	Source code for the application must be included, in the preferred form in which a programmer would modify it (no compiled binaries, no obfuscated code)
3.	No prevention of anyone from modifying the software and creating a derived work. Giving away or selling such derived works must not be prohibited or restricted, just as if the derived work were the original work.
4. No discrimination against any person or group of people is allowed. The license must not disallow the use of the software to make money or disallow it's distribution to foreign nationals, for example. 

## Common Licenses which are OSI-Certified

- Apache License 2.0
- BSD 3-Clause "New" or "Revised" license
- BSD 2-Clause "Simplified" or "FreeBSD" license
- GNU General Public License (GPL)
- GNU Library or "Lesser" General Public License (LGPL)
- MIT license

# The Garden of Open Source Licenses

There are a lot of open source licenses, (78 are currently certified by the Open Source Initiative) but the are often grouped into two categories, based on how they handle 'Generative Limitation'. Licenses which force derivative works to be licensed under the same license as the original are called 'copyleft'. Other licenses which permit relicensing, as long as the new license does not conflict with the old one, are non-copyleft. Non-copyleft licenses often allow closed-source derivative works, and copyleft licenses generally prohibit them. Both varieties allow commercial use of the licensed software, as long as a licensee does not attempt to assert exclusivity, and prevent others from equal opportunity to benefit commerically from the software.

# Non-Copyleft Licenses

## MIT License
This is one of the most simple licenses. It does only two things:

1. Releases all exclusivity rights, which normally are automatically given to the author of a work under the law, upon her completion of whatever the work is in a tangible form (e.g. an archive of source code files on the internet, or a git repository). This means that any other person which is not the author is allowed to, upon obtaining the code, sell or give it away, or modify it, or create a derivative work. __In particular, this license allows using the work in a closed-source product or creating a derivative work which is subject to a different license, as long as the original license is included as well__
2. Explicitly absolves the author of any legal responsibility for the consequences of use of the licensed software

## BSD license

The BSD license is essentially identical to the MIT license, with one additional requirement:

>"Neither the name of the <ORGANIZATION> nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission"

This is similar to the clause about warranty, in that it protects the authors from the uses the software may be put to, but in addition to legal protection, it protects their reputation from being exploited in connection with the software. This type of clause is called __non-attribution__.

## Apache License (version 2.0)
The 2.0 version is the most modern version of this license. The previous version (1.1) was very close to the BSD license.

Apache 2.0 is a longer and more explict license than MIT or BSD. It explicitly defines many of the implicit consequences of the MIT and BSD licenses and adds a few additional provisions for patent infringment, contributions to the original work which are covered under the same license, and what is and is not a derivative work.

The first major innovation in the Apache 2.0 license is a provision for 'upstreaming' or improvements made by people other than the original author, to be automatically included under the same license. This differentiates between contributions and derivative work, the latter of which can be relicensed, as long as the new license does not conflict with the Apache 2.0, wheras the former just becomes a part of the licensed work as long as the original authors accept it as such.

Apache 2.0 also explicity defines a 'Derivate Work'. Basically, if you can seperate the original from the work which is being considered as a 'Derivative Work', it's not a derivative work. This means that if you import or call a function from an Apache 2.0 licensed piece of software, but do not use it's source code as a part of your code, your work is not considered 'Derivative'. The rules for derivative works are:
1. They must explictly show in the source code what modifications were made.
2. They must include a copy of the original license and be subject to all of it's terms, but the derivative work creator may add additional terms to the license (this allows derivative works to be closed-source)

Apache 2.0 explicitly handles patent infringment, as well. Basically, it says that the license grants anyone who gets a copy of the software all of the patent rights that the author had, if any. It also has a provision that terminates the license and returns copyright with all of its legal protections to the originator if someone who has a copy of the software sues any person related to the software, providing further legal protection againt patent litigation.

# Copyleft Licenses

# GNU General Public License (the GPL)
The GPL is the most stringent of the copyleft licenses. 

It explicitly forbids any derivative work from being subject to any additional license clauses, and it interprets derivative works very broadly. Whereas the Apache license does not consider a program which imports or calls a function from an Apache licensed piece of software a derivative work, the GPL does. The GPL is sometimes referred to as 'contagious', meaning that any software that calls or uses functionality from a piece of software that is licensed under the GPL, is considered to be a derivative work, and must then be subject to all of the provisions of the GPL and only the provisions of the GPL. This ensures that any software that is distributed under the GPL cannot be made closed source, and cannot be used as a library in closed source programs.

The GPL differs from the Apache license in how it handles potential allegations of patent infringment against users or distributors of software licensed under it. The Apache license has a clause which renders the license void if someone who has the software initiates legal action against anyone else who has the software, which returns copyright protection to the author of the software. The GPL attempts to fight restrictive patent licencing by having a provision which says that if any court decision or ruling is made relating to a piece of software that is licensed under the GPL condradicts a provision of the GPL, then the only way to satisfy the ruling and the license is to discontinue distribution of the software. Basically this precludes anyone __including the original author__ from distributing the software or creating a derivative work, unless the original author relicenses the software. This has never been tested in court, and it's unknown if it's enforcible.

The GPL is the strongest license for a software author who belives that their software should always be distributed open-source.

# Lesser GNU General Public License (the LGPL)
The LGPL is similar to the GPL in many respects, except that it has a narrower concept of what constitutes a derivative work. In particular, it resembles the Apache license in classifying only works using substantial portions of the original code as derivative. A closed-source piece of software is allowed to call a function or use a subroutine from a LGPL-licensed piece of software without violating the license.

## References
Laurent, Andrew M. St. Understanding Open Source and Free Software Licensing. Accessed July 25, 2016. http://shop.oreilly.com/product/9780596005818.do.

