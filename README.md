# GID

*GID* defines a collection of `semantic symbols` that can be easily typed on most keyboards.
These symbols can be used to `extract the goal/aim/kind` of an idea and thereby `reduce linguisitc overhead` needed for its expression.
This is helpful for both `storing` and `retrieving` information quickly.

## Components

*GID* is made up of three components that build upon each other:
1) `Semantic Symbols`, which can be used as shorthand for their rough meaning.
2) `Semantic Compression` of notes by extracting their `goal/aim/kind` to a matching `symbol`.
3) `Level of Detail Hierarchy`, which can be used to break up larger ideas into smaller parts that get more specific/add detail to the respective parent level.

### Symbols

The associated meaning of each symbol is decidedly `vague`, balancing `specificity` with `flexibility`.
There also exists some overlap between some symbols, though their utilization might vary depending on the context.

```
>	    Note
.	    Side-Note
(..)	Relativation, side-note

<	    Counter-Point, Alternative
^	    Claim
°	    Idea

?	    Question
:	    Explanation
:=	    Definition
^=	    Equal Meaning
~	    Maybe / Approximation / Like
/	    opposite, difference
§	    Example
¬	    not  (AltGr+6)
!=	    not

i	    Info (some importance)
!	    Important
!!	    Very Important

0	    Goal/Aim/Focus
S	    Error / Problem
=	    Solution
x	    Condition

->	    Follow
=>	    Conclusion
<-	    Reason

1)	    Enumeration
--	    Option / Type
+	    Pro
-	    Contra

//	    (internet) source
$	    Command-example
>>	    Code-example
::	    Code-output
|-	    (Sub-)Directory

E	    parent
e	    is element of parent
00	    overview

*	    reference
#	    Inner-Document Reference
{TAG}	Tag
[AB]~	Abbreviation

d	    Date
v	    Location
@	    Person

**	    Comment
_	    Continued on next line
|	    Chain symbols
{..}	Inline side branch / Comment

[ ]	    TODO
[x]	    TODO - Done
[*]	    TODO - Active
[?]	    TODO - Unsure
[!]	    TODO - Priority
[p]	    TODO - Postponed
[~]	    TODO - Partly Finished / On Hold
[-]	    TODO - Closed / Deprecated
```


### Compression

By extracting some part of an idea into a `symbol`, you can `remove` all words that would otherwise be needed to specify that part.

Take for example the note
```
Peters claims that trees can walk when no one is looking (not sure if that is true).
```
which could be compressed to
```
^ Trees can walk when no one is looking {//|@ Peters} {? true}
```

### Level of Detail

Nesting notes into a `tree structure` is the core idea behind [outliners](https://en.wikipedia.org/wiki/Outliner).
Similar to the outline found in a book, writing in a tree allows you to `group` multiple aspect of an idea under a more general common point.
Like with a books `chapter, section, subsection, ...` hierarchy, this structure will allow you to easily `scan` the content of your notes on a high level, before `going deeper` into the `details` of the topic you are currently interested in.

If your text editor supports it, you can also collapse sub-trees, allowing you to hide away information that is not relevant at the moment.

This `parsability` is further improved by integrating the `semantic compression` via `symbols`, since the very first character of each point gives a hint to its content.

To get back to the previous example, one could write (among many options):

```
^ Trees can walk when no one is looking
  //|@ Peters

  [!] check other sources to confirm
```

or

```
^ Trees can walk _
  x no one is looking
  //|@ Peters

  ? is this true
    [!] check other sources
```

Of course, the degree to which you split larger ideas into nested branches is up to you.
Keep in mind that a very `high degree` of `nesting` and `compression` can make it `harder to reconnect` with your intended meaning at a later time, since the ambiguity of the `symbols` might not have enough `explicit context` to be resolved easily. 
Your `implicit context` during writing might not be present later!


## Benefits

I originally developed *GID* in the context of a part time job, university lectures and unstructured thinking sessions in the evening. So the following benefits result from my original requirements and experience with *GID* over the years.
You mileage with some of these points may vary, but they all result from improved `storage` and `retrieval` processes.

### Storage Speed

Similar to [stenography (shorthand)](https://en.wikipedia.org/wiki/Shorthand), reducing the amount of characters that need to be written significantly improves your speed.
This might come in handy when the subject of your notes is `moving quickly`.
(Think meetings, lectures, calls, interviews, fleeting ideas ...)
When your notes can keep up with the content, you tend to `miss less` of it.

Using *GID* might not speed you up much in the start; in fact it might even make you slower.
Since I just made up the symbols as I went and never had to learn them, the speed increase is one of the largest benefits for me personally.

In addition to compressed writing, the tree structure also helps here.
During particularly fast moving sections, it can be helpful to only briefly `touch on each point` and quickly move to the next one. Now the `structure` of the note will already be largely present, and the current implicit context can be made explicit by `filling in the gaps` once a pause presents itself.

### Retrieval Speed

Both `compression via symbols` and deep `nesting` can help you quickly retrieve specific information.
The `tree` structure of your notes will allow you to prune away large chunks of your notes during search.
By scanning the top most level, you might identify a few relevant points that point to general topics in their branches, and `exclude multiple large sub-trees`.
This can then be done recursively for each lower level.

Additionally, scanning the `symbols` at the start of each line, you might be able to `dismiss entire sub-trees` without even having to read the content of the point.
(E.g. a sub-tree that branches from an example for a point might not be relevant when you are looking for a definition to the parent of the example)

### Active Structuring

When you are not in a hurry, you can take your time to `think carefully` about the structure and symbol utilization of your notes.
Reasoning about what information can be `omitted`, and how it can best be `nested` can help you actively get a deeper `understanding` of the subject of your notes, while also making it easier to `decode` in the future.
In essence, you want to prepare a simple explanation for your future self (or other readers).

### Multithreading

In case you are presented with multiple `interleaving subjects`, it is helpful to `quickly locate` each thread.
This might happen if a previous point (e.g. in lecture/stream of consciousness/...) is brought up again at a later time.
Once the appropriate point has been found by flowing down from more general parents with the help of indicating symbols, the new information can be `included easily`.

### Transmission

For ideas that require more `continued thought` and work than can be achieved in one session, it is useful to try and capture ones mental state at the point of interruption.
The multitude of open tasks/thoughts/questions/... that accumulate during any sufficiently large project, can be offloaded in a `structured and iterative` manner (adding more detail as you go along).
This way the `highly connected` nature of our thoughts can be captured with a little `less loss` via a lower dimensional tree.
(As opposed to trying to capture the thoughts with even lower dimension of linear text).

You might e.g. use this when leaving work for the weekend or simply before going to bed with the intention of continuing in the next session.

Using *GID* deliberately (Active Structuring) can help you to `reconnect` with your thoughts in the future on re-reading your notes.


# Syntax Highlighting
In case you use VSCode, here is a rough text mate grammar that you can use:
https://github.com/ltOgt/GID-vscode
