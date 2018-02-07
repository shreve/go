Go
==

A stupidly simple link shortener.


## Usage

1. Add new links to `links.json`
2. Run `bin/gen`
3. Commit the changes
4. Upload to GitHub


## Setup

1. Fork this repo
2. Update `docs/CNAME` with your domain
3. Ensure GitHub Pages is enabled and is looking at `/docs`
4. Create a CNAME DNS record from your domain to {username}.github.io


## Notes

`links.json` contains an object where the keys are the shortened paths and the
values are the destination.

`bin/gen` is written in ruby. It doesn't require an extra dependencies outside
the standard library, and should be compatible with versions as old as 1.8. It
has only been tested on versions above 2.2.

The root of the domain will be handled by the link with path `this`.
