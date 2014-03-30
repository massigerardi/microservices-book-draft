1. An introduction
==================

- Prologue
- Architectures
- SOA
- Microservice Architecture
- Dropwizard, Spring Boot
- Polyglot persistence and languages
- Platforms as a Service
- Software as a Service

## Prologue

> Divide et impera

A spectre is haunting present architecture design.

But, differently from the spectre of early 20th century, no one is entered in a holy alliance to exorcise it.
No pope, no tzar, no Metternich and Guizot.

On the contrary the software development community is more and more embracing the new concept of microservices.

And why this should not occur? Microservices seems to offer at the moment undeniably advantages in terms of software architecture and in software development.

Scope of this book is to give an insigth into this new approach and to provide a working example of microservices in the real world.


## Architectures

Traditionally, architecture are build in a three tiers fashion: a client side, a database and a server side.

![3-tiers architecture](images/3tier.jpg)

Client side applications usually consist of a set of HTML pages and javascript libraries, handled by a browser and defining the user interface, what the actual user sees and uses.

Databases, on the other hand, provided the basic data to populate and control the HTML layer; usually traditional databases, mostly relational, consist of variuos tables managed by a common database management system.

In the middle of the previuos two tiers, lay the server application, responsible to handle any request from the client side, run any business logic to retrieve, update and combine the data coming from the database into a HTML views.

We will focus out attention on this last component.

###Unix philosophy

```
MG: review the wording
```

__Modularity__: Developers should build a program out of simple parts connected by well defined interfaces, so problems are local, and parts of the program can be replaced in future versions to support new features. This rule aims to save time on debugging complex code that is complex, long, and unreadable.

__Clarity__: Developers should write programs as if the most important communication is to the developers, including him- or herself, whom will read and maintain the program rather than the computer. This rule aims to make code readable and comprehensible for whoever works on the code in future.

__Composition__: Developers should write programs that can communicate easily with other programs. This rule aims to allow developers to break down projects into small, simple programs rather than overly complex monolithic programs.

__Separation__: Developers should separate the mechanisms of the programs from the policies of the programs; one method is to divide a program into a front-end interface and back-end engine that interface communicates with. This rule aims to let policies be changed without destabilizing mechanisms and consequently reducing the number of bugs.

__Simplicity__: Developers should design for simplicity by looking for ways to break up program systems into small, straightforward cooperating pieces. This rule aims to discourage developers’ affection for writing “intricate and beautiful complexities” that are in reality bug prone programs.

###Monolithic architecture

> __monolithic__
>
> _mɔnəˈlɪθɪk_
> 
> adjective
>
> 1. formed of a single large block of stone.
> 2. (of an organization or system) large, powerful, indivisible, and slow to change.


Usually the server side component of a 3-tier architecture is a large _monolithical_ beast, self contained, where all our logic processes occurs and are executed.
The first term that comes to mind when talking of monolithic is megalithic. 

> __megalithic__
>
> _mɛgəˈlɪθɪk_
>
> adjective 
> 
> 1. relating to or denoting prehistoric monuments made of or containing megaliths

I would rather use the term _megalithic_ to point my finger to such architectures, at it better express one of the weakness of them: monolithic architectures tend to grow, to a point where they become too big.
Moreover, by becoming big they also tend to grow old faster and to offer more and more resistance to change.

_A megalithic system is what you get when a monolithic system grows in functionality and interdependence at the same time._ [<< MG >>: reword definition - from [http://c2.com/cgi/wiki?MonolithicDesign](http://c2.com/cgi/wiki?MonolithicDesign)]

Megalithic is large, great, big and at the end history. Think Stonehenge with a database plugged in.

Storically, monolithic architectures are a sort of natural way to design a complex structure: provided a consistent domain, all the logic is concentrated in a single processing unit. 
Before distributed system, each application needed to be self contained. Everything (data, processing power, processing definition, user interface) had to be available there.

Taking to the extreme, we could say that historic monolithic system are actually a good definition of lack of architecture and of architects.

A non-distributed monolithic system needs no architecture because has no process boundaries.
Internal components communicate within the process, so there is no need to define and maintain interfaces between components. 

Monolithic architecture are found in lot of enterprise solutions. 


```
MG
    μέγα- (mega-) great, big, large
    μόνο- (mono-) one
    πολυ- (poly-) several, many
    λίθος (lithos) stone
play word: take a birds with a few stones.
```


## SOA
## Microservice Architecture
## Dropwizard, Spring Boot
## Polyglot persistence and languages
## Platforms as a Service
## Software as a Service
