# But, Andreas, why?

Author Cory Doctorow is a cultural sharing activist, and has released all his books since 2003 with open licenses – it is a political decision that gives him "artistic, moral and commercial satisfaction", but also something he believes leads to increased sales and distribution of his books.

The book **"Little Brother"** was previously released in Nynorsk by the publisher Samlaget as **"Veslebror ser deg"** ("Little Brother is Watching You") in 2009. The book was well translated by **Øystein Vidnes**, which earned him the Ministry of Culture's Translator's Prize the same year.

Unlike some other releases in other countries, Samlaget's translation was not published with Creative Commons licenses – however, they first released half the book for free online at [veslebrorserdeg.com](https://web.archive.org/web/20100104043824/http://www.veslebrorserdeg.com) (Wayback Machine link from early 2010), and the rest only upon direct request, before they released the entire book for free after pressure from the author and nerds in Norway.

But it didn't take long before the domain died out, and access to the book was gone – and today the only way to read the book is to borrow it through a library service, buy it second-hand, or get the PDF file sent from another fan. I get happy when culture intended to be in the open is allowed to be in the open, and I was very annoyed when the Norwegian translation's digital footprint disappeared.

The domain [veslebrorserdeg.com](http://www.veslebrorserdeg.com) was available, so I bought it. I wanted to make the book freely available electronically again, but I didn't dare to upload Samlaget's PDF. In a conversation with Thomas Brevik, I was reminded that the Creative Commons license allows for derivative works, like translations, as long as they are released under the same license.

So, [this is my translation](/02-boka/01-Kapittel1.md), partly supported by machine learning with me as editor and proofreader. It is not as good as Vidnes's, but it exists, it is freely available, and it is released under the same license as the original. If Samlaget wishes to get their original translation out into the world, this space is readily available.

"Little Brother" is a an entertaining pageturner with a nerdy slant. But what I think it does best is to — even before surveillance capitalism really took off — be a quick introduction to the work against oppression in an increasingly digitalized world, and it is still strikingly relevant, probably even more so now than when it was released.

As Doctorow himself writes in the [introduction](/01-intro/02-intro.md):

    "This book is meant to be something you do, not just something you read."

## But, Andreas, how?
Kvefsebol (Hornet's Nest) Press is a name I had picked out in case I wanted to publish RPG adventures online, but this book got there first. This business is strictly noncommercial. If you want to pay someone for something, buy a Doctorow book, or [check if you can donate copies of the book to a teacher](https://craphound.com/littlebrother/donate/). 

This page is built from a long line of markdown files which I am trying to read through. Through [JupyterBook](https://jupyterbook.org/en/stable/start/build.html) I have made searchable HTML-pages of the files, published on [Github](https://github.com/tanketom/veslebrorserdeg) with [ghp-import](https://github.com/c-w/ghp-import).

Now, when I update one of my markdown files, I open Terminal, navigate to the parent folder, and type:

```
jupyter-book build veslebrorserdeg/
```

Then:

```
cd veslebrorserdeg
ghp-import -n -p -f _build/html
```

Then Github hopefully handles the rest!

For now, the PDF is made by sending a collected markdown file of the book to a Word file with this commando from the parent folder of the project.

```
find . -name '_build' -type d -prune -o -name "*.md" -print | sort | xargs pandoc -o combined-document.docx
```