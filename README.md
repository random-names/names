# names

A collection of database for generating random names. Currently hosts the following database:

- census-90: An English-name database. Collected from [https://github.com/treyhunner/names](https://github.com/treyhunner/names).
- heroku: A Heroku-like database, includes adjs and nouns.

### Database structure

A most basic example is [heroku](https://github.com/random-names/names/tree/master/heroku), with just names placed in differernt lines, which means that every word in the database has the same percentage to be picked.

Next comes the example with different percentages in [census-90](https://github.com/random-names/names/tree/master/heroku). You can easily find out that every word is followed by a float number, which is the cumulative percentage of all the names occured until current line. That is to say, the number in the last line  of the file is usually 100. I say usually is because the database may not contains all the names sometimes. Just take census-90 as an example, it doesn't include some rare names.