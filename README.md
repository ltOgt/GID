# GID

GID defines a collection of ascii symbols that have some general meaning.

For example `?` for a question, `:=` for a definition, `:` for an explenation, `>` as a general point and `<` as a counter point.<br>
(A list of all symbols along with their rough meaning can be found further down.)

These symbols can be used to change the structure of your notes.
Preceeding a bullet point (or larger text) with a semantic symbol has two benefits:
(1) Its word count can often be reduced, and (2) the beggining of the line gives a hint at its content.
This leads to both improved note taking speed and improved parsability of the resulting note tree.

By nesting points via indentation, you can break up longer sentences into multiple levels of shorter ones.
This again exposes more line beginnings to be filled with symbols describing the smaller pieces.
Additionaly a level of detail hierarchy can be gained.

The extend to which you break up the tree is up to you.

## Goals

### Take notes quickly
Reducing word count can help you stay on track when the subject of your notes is moving fast.
This might happen in meetings, lectures, calls or for fleeting ideas that cant wait to slip your mind.

### Jump back and forth
If you want to take notes on multiple subjects at once, it is helpful to be able to quickly locate each thread to extend it.
This might happen if a previous point (e.g. in lecture/stream of conciousness/...) is brought up again at a later time.

### Store and Restart
For ideas that require more continued thought and work than can be achieved in one session, it is useful to try and capture ones mental state at the point of interruption.
This might happen at work when you leave for the weekend (holiday/tomorrow), during a larger project, or simply before going to bed.

## Symbols
Here are the symbols I use most often.
The meaning behind them is decidedly vague, so that they can be flexible but still useful.
There also exists some overlap between some symbols.

```
`>`     Note
`.`     Side-Note
`(`     Relativation, side-note  `)`

`<`     Counter-Point, Alternative
`^`     Claim
`°`     Idea

`?`     Question
`:`     Explenation
`:=`    Definition
`^=`    Equal Meaning
`~`     Maybe / Approximation / Like
`/`     oposite, difference
`§`     Example
`¬`     not  (AltGr+6)
`!=`    not

`i`     Info (some importance)
`!`     Important
`!!`    Very Important

`0`     Goal/Aim/Focus
`S`     Error / Problem
`=`     Solution
`x`     Condition

`->`    Follow
`=>`    Conclusion
`<-`    Reason

`1)`    Enumeration
`--`    Option / Type
`+`     Pro
`-`     Contra

`//`    (internet) source
`$`     Command-example
`>>`    Code-example
`::`    Code-output
`|-`    (Sub-)Directory

`E`     parent
`e`     is element of parent
`00`    overview

`*`     reference
`#`     Innerff-Document Reference
`{TAG}` Tag
`[AB]~` Abbreviation

`d`     Date
`v`     Location
`@`     Person

`**`    Comment
`_`     Continued on next line
`|`     Chain symbols
```


# GID example version of this file
```
> GID
  := collection of semantic ascii symbols
    § '?' Question
    § ':=' Definition
    § '>' General Point
    § '<' Counter Point
    ** full list further down

  ! GID was mainly developed in the context of node trees
    (|: notes nested via indentation )
    . can also just be used in normal text, sticky notes, ...

  1) extract rough ~meaning of thought by selecting a matching symbol
  2) place symbol at beggining of sentence (or text)
  3) write note concisely

  + reduce word count
  + line start hints at content

  ->|+ Faster Note Taking
  ->|+ Faster Note Parsing

  -- using nested note trees
    ->|+ break up into levels of detail
    ->|+ more reduction via symbols
    
    ( can use this a lot or a little, depending on taste )
    
  0 Take notes quickly
    S subject of your notes is moving fast
        §|<- Dont loose track in fast meetings/lectures/calls/...
        §|<- Capture fleeting ideas
    = Reduce Word Count
      => Less time wasted writing

  0 Jump back and forth
    S multiple parallel threads
        §|<- Return to previous points in meetings/...
        §|<- stream of conciousness

    = Improve Parsability
      => Quickly find previous points
    
  0 Store and Restart
    S Size of idea too large for one session
        §|<- Leaving work for weekend/tomorrow/...
        §|<- Going to bed

    = Reduce Word Count and Use Branching Notes
      => Capture multiple open tasks and ideas quickly
    = Improve Parsability
      => Connect with previous state 
```
