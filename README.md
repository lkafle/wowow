# wowow

Everybody loves :sparkles: **Lava dai** :sparkles:, specially his streams of **w(ow)*** in internet.

Nobody can decipher it till date, Why not make a *compiler* for it?

**************

***yes!*** **Welcome Abroad**

###### Post you thought! in [issues](https://github.com/haude/wowow/issues/new)

For those who don't have **Github** make one [here][github] or use [etherpad][1]

**************

:warning: ***Warning: this article contain bit mathematics, please be careful while editing***

##lava language

	A lava language L over an alphabet Σ is a subset of Σ*, that is, a set of words  over that alphabet.
	Sometimes the  sets of  words are grouped into  expressions, whereas rules  and  constraints may be
	formulated for the  creation of 'well-coded expressions'.

Following rule describes a language **L** over the alphabet **Σ={w,o,+,!}**
> * There cannot not empty **L**. *(L ≠ ∅)*
> * The first letter is always starts from **w**. *(^w)*

### :one: Construction
For lava languages one can explicitly enumerate all well-formed words.
For example, we can describe a language **L** as just 

>**L = {'wow', '+1', 'like', 'blessed', 'wonderful'}**

However, even over a regular alphabet such as **Σ = {w,o}** there are infinitely many words:
> "wo", "wowo", "wowow", "wowowwowow", ….

Therefore formal languages are typically infinite, and describing an infinite lava language is not as simple as writing L = {"w", "wowo", "wowow"}.
Here are some examples of lava languages:

> **L = Σ***, the set of all words over **Σ**;
> **L = w{"wo"}* = {"w"n}***, where n ranges over the natural numbers and "wo"n;
> a set of syntactically correct statement can give programming language which can be defined by a context-free grammar

### :two: Context-free grammar (CFG)

In *lava language theory*, a *context-free grammar* (CFG) is a formal grammar in which every production rule is of the form
> **V → w**

where,
> * **V** is a single nonterminal symbol,
> * **w** is a string of terminals and/or nonterminals (w can't be empty).

The languages generated by context-free grammars are known as the context-free languages.

#### Formal Defination
A context-free grammar **G** is defined by the 4-tuple:

**G = (V, Σ, R, S,)**

where,
> * **V**, is a finite set; each element **v ∈ V** is called a non-terminal character or a variable. Each variable represents a different type of phrase or clause in the sentence. Variables are also sometimes called syntactic categories. Each variable defines a sub-language of the language defined by **G**
> * **Σ**, is a finite set of terminals, disjoint from **V**,, which make up the actual content of the sentence. The set of terminals is the alphabet of the language defined by the grammar **G**
> * **R**, is a finite relation from **V**, to **(V ⋃ Σ)***, where the asterisk represents the Kleene star operation. The members of **R**, are called the (rewrite) rules or productions of the grammar
> * **S**, is the start variable (or start symbol), which is in most case be **w**

### :three: Grammar Production Rule

In the context of formal language theory, something is called **"regular"** when it has a grammar where all production rules have one of the following forms:

	B → a
	B → aC
	B → ε

You can read those → rules as *"The left hand side can be replaced with the right hand side"*. So the first rule would be *"B can be replaced with a"*, the second one *"B can be replaced with aC"* and the third one *"B can be replaced with the empty string"*.

	By convention, 
	uppercase characters denote "non-terminals" - symbols which can be broken down further
	lowercase characters denote "terminals" - symbols which cannot be broken down any further

[1]:http://openetherpad.org/hFHmRx8tDD
[2]:http://m.c.lnkd.licdn.com/mpr/mpr/shrink_200_200/p/3/000/1f7/264/0ac820f.jpg
[github]:https://github.com/signup/free


