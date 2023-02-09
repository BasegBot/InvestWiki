# InvestWiki

The toffee wiki repo!

## Usage

Within the `./wiki` directory, each subdir corresponds to an actual path on the website.

For example, `./wiki/home/[lang].md` gets translated to `/wiki/[lang]/home` when built on the server, where lang is replaced with the browser's language code (or whatever's manually specified).

### Relative links

Use the relative directory structure present in the repo. The site will parse the language for you through its middleware.

If you're currently on the page (directory) `/wiki/bot`:

`usage` will correspond to `/wiki/bot/usage` (you can also specify `/wiki/bot/usage`) directly if you wish.

**However, do not end the relative URL with an ending slash** as you'll see in a second.

### Direct links

#### Internal

If you want to link to a specific internal link, end the URL with an ending slash!

`/ranking/` links to the ranking page on the site
`/wiki/ja/home/` directly links to the Japanese version of home

#### External

Just link as you normally would with the `https` prefix. It should not be needed to add the domain to the `next.config.js` as we aren't using its optimizer for markdown images.

### Images

#### Internal

Conventionally, store images you'd like to use in a folder called img within the same subdir and refer to them relatively.

`img/image_name.webp`

Using a starting slash will refer to it as a absolute/direct path, so if you need to refer to another image in different page, just prefix the entire path with `/img`

`/img/wiki/bot/img/image_name.webp`

#### External

Same as for links!

## Contributing

tbd (?)
