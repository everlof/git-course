### Intro

###### Innehåll idag:

- Kort historia git och versionshantering
- (Övning: Installera git & Sourcetree)
- Grundläggande kommando
- Övning: Skapa ett repo, lägg in en fil och commita
- Övning: Hämta ut ett repo från github
- Övning: Gör en ändring till repot som checkades ut
- Övning: Identifiera när en "bug" introducerades

###### Vad är versionshantering?

Records changes to files over time, so that you can recall specific versions later.

###### Varför använder vi versionshantering?

Tracability

###### Grundläggande terminologi

Filerna "bor" i ett **repository**.

Ett **repository's** historik består av **commits**.

En **commit** består av:

- Datum
- Författare
- Ett meddelande som beskriver **commiten**
- En ögonblicksbild av "filträdet" vid **commit**-tillfället

###### Vilka typer av verktyg finns det?

VCS vs. DVCS

###### Advantages of DVCS (compared with centralized systems) include:

- Allows users to work productively when not connected to a network.
- Common operations (such as commits, viewing history, and reverting changes) are faster for DVCS, because there is no need to communicate with a central server.[5] With DVCS, communication is only necessary when sharing changes among other peers.
- Allows private work, so users can use their changes even for early drafts they do not want to publish.[citation needed]
- Working copies effectively function as remote backups, which avoids relying on one physical machine as a single point of failure.[5]
- Allows various development models to be used, such as using development branches or a Commander/Lieutenant model.[citation needed]
- Permits centralized control of the "release version" of the project[citation needed]
- On FOSS software projects it is much easier to create a project fork from a project that is stalled because of leadership conflicts or design disagreements.

###### Disadvantages of DVCS (compared with centralized systems) include:

- Initial checkout of a repository is slower as compared to checkout in a centralized version control system, because all branches and revision history are copied to the local machine by default.
- The lack of locking mechanisms that is part of most centralized VCS and still plays an important role when it comes to non-mergeable binary files such as graphic assets or too complex single file binary or XML packages (e.g. office documents, PowerBI files, SQL Server Data Tools BI packages, etc.).[citation needed]
- Additional storage required for every user to have a complete copy of the complete codebase history.[6]
- Increased exposure of the code base since every participant has a locally vulnerable copy.[citation needed]


VCS:

- CVS (1986)

- Subversion (SVN) (2000)

DVCS:

- BitKeeper (2000, OS 2016)

- GIT (2005)

- Mercurial (2005)

###### Kort historia GIT

Linuxkärnan email-patchar 1991-2002.

BitKeeper 2002.

In 2005, the relationship between the community that developed the Linux kernel and the commercial company that developed BitKeeper broke down, and the tool’s free-of-charge status was revoked. This prompted the Linux development community (and in particular Linus Torvalds, the creator of Linux) to develop their own tool based on some of the lessons they learned while using BitKeeper. Some of the goals of the new system were as follows:

- Speed
- Simple design
- Strong support for non-linear development (thousands of parallel branches)
- Fully distributed
- Able to handle large projects like the Linux kernel efficiently (speed and data size)

Since its birth in 2005, Git has evolved and matured to be easy to use and yet retain these initial qualities. It’s amazingly fast, it’s very efficient with large projects, and it has an incredible branching system for non-linear development (See Git Branching).

Det är ju kul att vi kan gå tillaka i tiden! Här kan vi titta på de ändringarna som gjordes på git själv.

https://github.com/git/git/commits/master?after=d4a392452e292ff924e79ec8458611c0f679d6d4+60739&branch=master

First commit: 

https://github.com/git/git/commit/e83c5163316f89bfbde7d9ab23ca2e25604af290#comments

### Övningar

##### 1. Installera git ("Git Bash")

https://git-scm.com/downloads

