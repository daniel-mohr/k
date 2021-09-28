# Pandoc Markdown Demo {#sec:first}

Put your bibliography into `literature.bib`.

Your markdown files are processed in alphabetic order.

In this section we will see what you can do with Markdown.

## Some simple formatting

We can write in *italic*, **bold**, `monospace` and ~~strike-through~~.

We can use sub- and superscripts, like: H~2~O and  2^10^ is 1024.

Some inline LaTeX-style math -- $f(x)=x^{\sqrt{2}}$ -- and also display math:

$$
e^{i\pi} -1 = 0
$$

## Referencing

We can link to [external sites](https://www.startpage.com).

We are now in the [first section](#sec:first) and see what is possible.

Nameless links: <https://google.com> and <sam@green.eggs.ham>
[Write me!](mailto:sam@green.eggs.ham)

This is a proper citation [@wilkinson2016fair].

Here is a a footnote reference[^somenote].
Here is an inline note.^[Inlines notes are easier to write, since
you don't have to pick an identifier and move down to type the
note.]

[^somenote]: This is another note.

This paragraph won't be part of the note, because it isn't indented.

## Quoting

> This is a block quote. This
> paragraph has two lines.
>
> 1. This is a list inside a block quote.
> 2. Second item.

> This is a block quote.
>
> > A block quote within a block quote.

Some code

    if (a > 3) {
      moveShip(5 * gravity, DOWN);
    }


More code

~~~~~~~
if (a > 3) {
  moveShip(5 * gravity, DOWN);
}
~~~~~~~

```python
def test():
  println("hello world!")
```

Preserve manual spacing:

| The limerick packs laughs anatomical
| In space that is quite economical.
|    But the good ones I've seen
|    So seldom are clean
| And the clean ones so seldom are comical

## Various kinds of lists

A tight list 

* one
* two
* three

A loose list

* First paragraph,
  
  continued.

* two

* three

A nested list:

* fruits
  + apples
    - macintosh
    - red delicious
  + pears
  + peaches
* vegetables
  + broccoli
  + chard

An ordered list:

1.  one
2.  two
3.  three

With manual number styling:

9)  Ninth
10)  Tenth
11)  Eleventh
       i. subone
      ii. subtwo
     iii. subthree

A task list:

- [ ] an unchecked task list item
- [x] checked item

# Definition lists

Term 1

:   Definition 1

Term 2 with *inline markup*

:   Definition 2

        { some code, part of Definition 2 }

    Third paragraph of definition 2.


Term 3
  ~ Definition 3

Term 4
  ~ Definition 4a
  ~ Definition 4b


(@good)  This is a good example.

We can refer to our example (@good) which illustrates, ...

A horizontal rule:

----

## Tables

  Right     Left     Center     Default
-------     ------ ----------   -------
     12     12        12            12
    123     123       123          123
      1     1          1             1

Table:  Demonstration of simple table syntax.

Or without header:

-------     ------ ----------   -------
     12     12        12             12
    123     123       123           123
      1     1          1              1
-------     ------ ----------   -------

Or with multiple lines:

-------------------------------------------------------------
 Centered   Default           Right Left
  Header    Aligned         Aligned Aligned
----------- ------- --------------- -------------------------
   First    row                12.0 Example of a row that
                                    spans multiple lines.

  Second    row                 5.0 Here's another one. Note
                                    the blank line between
                                    rows.
-------------------------------------------------------------

Table: Here's the caption. It, too, may span
multiple lines.


: Sample grid table.

+---------------+---------------+--------------------+
| Fruit         | Price         | Advantages         |
+===============+===============+====================+
| Bananas       | $1.34         | - built-in wrapper |
|               |               | - bright color     |
+---------------+---------------+--------------------+
| Oranges       | $2.10         | - cures scurvy     |
|               |               | - tasty            |
+---------------+---------------+--------------------+

Colons mark alignment:

+---------------+---------------+--------------------+
| Right         | Left          | Centered           |
+==============:+:==============+:==================:+
| Bananas       | $1.34         | built-in wrapper   |
+---------------+---------------+--------------------+

For headerless tables, the colons go on the top line instead:

+--------------:+:--------------+:------------------:+
| Right         | Left          | Centered           |
+---------------+---------------+--------------------+


| Right | Left | Default | Center |
|------:|:-----|---------|:------:|
|   12  |  12  |    12   |    12  |
|  123  |  123 |   123   |   123  |
|    1  |    1 |     1   |     1  |

  : Demonstration of pipe table syntax.


