# TEENY SERVER

When I do any small-scale front-end work without the benefit of some framework's
prewritten server, it's handy to be able to run a little non-caching server that
pops your current directory onto localhost. This is a short ruby script to do
exactly that. Just run `serve` from the command line in your project directory,
and you'll be up and running. To stop the server, send it an interrupt signal
with control-c.

The default server is at port 1234, because typing that into a URL bar is really
easy on the fingers, but if you provide a different port as an argument to the
script, it'll use that instead.  

## COOL, NOW HOW DO I INSTALL THIS SUCKER

I'm assuming you want to be able to run this in any directory like a normal
command-line utility. If you want something fancy and custom, nice! I just can't
help.

##### Stuff You Need
* You need a `ruby` executable on your system. If in doubt, try `which ruby`.
* You need a directory in your PATH you can stick this in. If you're not
  comfortable messing around with read-only system folders like `/usr/bin` or
  `/usr/local/bin`, this little one-liner gets you set up the same way I am:
```sh
mkdir ~/.bin && PATH=$PATH:~/.bin && echo "export PATH=$PATH:~/.bin" >> ~/.zshrc
```
Or bashrc or whatever.

##### Stuff You Do
* Clone the repo wherever makes sense to you, and `cd` into that directory
* Make the script executable with `chmod +x serve`
* Symlink to the script from somewhere in your $PATH with `ln -s /absolute/path/to/teeny_server/serve ~/.bin`.
* Have yourself a nice day.

### BIBLIOGRAPHY

[a blog post](http://tobyho.com/2009/09/16/http-server-in-5-lines-with/).
