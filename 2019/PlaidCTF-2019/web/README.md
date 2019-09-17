# Web

## Potent Quotables

Web (300 pts)
I set up a [little quotes server](http://quotables.pwni.ng:1337/) so that we can all share our favorite quotes with each other. I wrote it in Flask, but I decided that since it's mostly static content anyway, I should probably put some kind of caching layer in front of it, so I wrote a caching reverse proxy. It all seems to be working well, though I do get this weird error when starting up the server: 

```
* Environment: production

    WARNING: Do not use the development server in a production environment.

    Use a production WSGI server instead.
```

I'm sure that's not important. 

Oh, and don't bother trying to go to the /admin page, that's not for you.

Hint: Extra server

Alternate server for PQ: `http://quotables2.pwni.ng:1337/` (same configuration in all respects)

## Triggered

Web (280 pts)

I stared into the abyss of microservices, and it stared back. I found something utterly terrifying about the chaos of connections. 

"Screw this," I finally declared, "why have multiple services when the database can do everything just fine on its own?" 

And so on that glorious day it came to be that everything ran in [plpgsql](http://triggered.pwni.ng:52856/).