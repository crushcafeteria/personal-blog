# Blogging with Markdown

<div class="author">
	Written by Nelson Ameyo, 2nd May 2015
</div>
---

During our 80/20 TGIF Friday last week at [Deveint Limited](http://deveint.com), my CT0, [Prof](http://nandaa.com) perked my attention to an Github project called [MkDocs](https://github.com/mkdocs/mkdocs). According to the author of MkDocs [Tom Christie](https://twitter.com/_tomchristie):-


> MkDocs is a fast, simple and downright gorgeous static site generator that's geared towards building project documentation.

It is build with Python and it summarily creates beautiful HTML documentation websites from MarkDown files. Personally, I have been unsatisfied with blogging and software documentation software. I needed a new and lazy way to write stuff for the Internet easy or just create some solid docs to ship with our ready software. Word documents couldn't just cut it. 

Open source systems like MediaWiki or Wordpress are effective, but sometimes they are overkill for simple projects. Think killing a rat with an M-16. Hell, I even developed me a simple PHP-MySQL thingy powered by the [CodeIgniter Framework](http://codeigniter.com). I didn't like my solution any better. What I needed was something that could hit the groun running, no DB setups, <code>var_dump()</code> or app configurations. Something that I can just render once and run anywhere.

## How MkDocs works
MkDocs is easy to work with. It stays out of your way as you write pages. If you do not have Python installed, go ahead and follow installation instructions on the [Python Website](https://www.python.org/). You can test if you got Python installed by typing this in your shell:-

```shell
python --version
```

Go ahead and install <code>pip</code> if you don't have a copy. Click [here](https://pip.pypa.io/en/stable/installing.html) for <code>pip</code> installation instructions.

Creating a new MkDocs project is easy peasy. cd into your favorite directory and type this into your shell:-

```shell
mkdocs new [project-name]
```

This command creates an empty MkDocs project in that folder. You can not open the <code>docs</code> folder and add your MarkDown files here. An <code>index.md</code> file has already been created for you. Go ahead and edit it. MkDocs comes with a really cool server that supports autreloading. This means every time you make changes to your MarkDown files, you can preview the changes you make live in the browser. To start the MkDocs server, cd into the MkDoc project root and type:-

```shell
mkdocs serve
```
You will see a message:

```
Serving on http://127.0.0.1:8000
```

Cool! You are now up and running. You can follow the address to view your freshly pressed MarkDown HTML site. You can render all your MarkDown files by entering this in your shell:-

```shell
mkdocs build
```

This command will render a full HTML website into the <code>sites/</code> folder. You can then upload this folder to your file hosting and setup a domain, if needed. See how it's easy? No databases, no config files, no environments. In case you make an update to your MkDocs project, you simply build it again and re-upload.

## Extending MkDocs to blogging
I loathe wasting bytes. WordPress is awesome. But really, how many features do you get to use as a 'small-scale' blogger? I'd guess 40% maybe? Your consumers are looking for content. MkDocs gets content to the consumer much more easily than other tools. Here is my setup in using MkDocs as a blogging platform.

### Categorizing posts
I have grouped my posts into month-year folders e.g. may-2015, june-2015. This also applies to images I upload to the blog.

### File Naming conventions
I have used dashes to separate words in file names. The advantages of this method is you create a more unique file name which reduces the chances of duplicates in one folder and it also produces clean URLs, which you will definitely want if you wish Google and other search engines to desire you.

## Conclusion
That is it for MkDocs. If you wish to learn more, you can check out their awesome website at [mkdocs.org](mkdocs.org). An do not forget to use Git to maintain a history of your blog. It will really be a plus when you content has really grown 5 years down the line.
