# TEENY SERVER

When I do any small-scale front-end work without the benefit of some framework's
prewritten server, it's handy to be able to run a quick little non-caching server
to pop your current directory onto localhost (I use port 1234 because it's nice
and ergonomic to type, but it's trivial to change if you want a different one).

## WHAT YOU EVEN GOT HERE, MISTER, SPIT IT OUT

A short ruby script that kicks up a server in your current working directory.
Just clone the repo somewhere, and assuming you want to be able to just run it
any old where as a command line utility, `cd` into the repo and run
`chmod +x serve && ln -s absolute/path/to/teeny_server/serve somewhere/in/$PATH`.
The whole script was (only barely) adapted from [a blog post](http://tobyho.com/2009/09/16/http-server-in-5-lines-with/).
