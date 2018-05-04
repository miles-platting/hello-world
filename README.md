## Hello world

I'm a 70 year old, retired and getting back into the programming activity to try to keep my brain ticking. How things have changed over the last 40 years!

My introduction to github has been cloaked in a large degree of bafflement. What are all these things? pushes and pulls and commits and adds and HEADS and what all? I get the general idea but I am still finding the terminology and the actions quite obscure at present.

This first entry just looks at how you get started assuming you have a github account and you are bamboozled by the jargon and the order of github thngs.

So these are the steps I took:

git commit -m "README additions step 1"

Quite what that has done I don't know yet. I didn't see anything significant happening so perhaps some background prep has occurred.

It seems that the steps are:

1. Make the changes to a file duh edit a file
2. do the  git commit -m "These are my remarkable changes" -a
3. git push

then put your user name and password in.

Must get markdown magic symbols sorted.

So what's the best way (so far) to use github with your software projects?

1. Make a directory/folder which contains your source code.
2. Create a .gitignore file. This will contain a list of all the file patterns and names that you don't want on github.
3. Learn how to use MarkDown (md files), yet another syntax. Visit [daring fireball](https://daringfireball.net/projects/markdown/basics) for more info.
4. Get au-fait with Makefiles and make, CMake too if you have the time.

Later I'm going to add a how-to-actually-get-started-with-a-project, you know using git locally to manage the project then when it is past the getting-going stage I'll github it. Can github be used as a verb? I'll be githubbing and expect that the project will have been githubbed in due course. 

##Creating a new project

I have a folder called modelling and in there it looks like this:

<pre>
drwxr-xr-x    7 dev  staff   238  4 May 16:23 .
drwxr-xr-x+ 188 dev  staff  6392  4 May 13:57 ..
-rw-r--r--@   1 dev  staff  6148  4 May 13:05 .DS_Store
drwxr-xr-x    5 dev  staff   170  4 May 16:25 hello-world
-rw-r--r--    1 dev  staff     0  4 May 13:28 master
drwxr-xr-x    7 dev  staff   238  4 May 12:48 model-building
drwxr-xr-x    3 dev  staff   102  4 May 16:25 sqlite-lite
</pre>

There is a hello-world project, a model-building project and an sqlite-lite project. The latter is a newbie and I will create a git structure in there, add the code etc, test it and finally send it off to github. There's a master file with nothing in it, I guess that is a git artefact. And there's the ubiquitous .DS_Store, another darned artefact of computing. You can hide the buggers but it's not worth the trouble and if you delete them you will probably lose some of the folder viewing properties  or something else useful. Anyway enough of this grumbling, although why the bloody things can't be hidden by default I don't know.

###The sqlite-lite project

A loose wrapper, if that's the correct term, for working with an sqlite database. You must surely know about Sqlite, the creation of Dr. Richard Hipp, and if don't know you should look it up. Sqlite is written in C and so far as I can tell it can run anywhere and like all thorough-breds it can run on the smell of an oily rag. Sqlite is one of those tools, like a good text editor, that is a mainstay of programming.

There are many good Sqlite libraries around and Sqlite has been wrapped and bundled all kinds of ways. This wrapper is simple but effective and can be used by dropping the code straight in to your own code if you are using C++, or you can use it as a library, archive style. See the sqlite-lite repo for more.