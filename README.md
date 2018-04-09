# gitbook-plugin-open-graph

Adds open graph and twitter sharing meta information to `<head>`

## Installation

    npm install gitbook-plugin-open-graph

## Usage

add to `book.json`

```
{
  "plugins": [
    "open-graph"
  ],
  "pluginsConfig": {
    "open-graph": {
      "baseURL": "http://example.com"
      "defaultDescription": "This is my default share description",
      "defaultImage": "images/default-share.jpg"
    }
  }
}
```

## Open graph titles, descriptions and images

By configuring a default description and image, every page will have that image associated with it when being shared on twitter or facebook.

You can customize any page's share title, description and image in the book by using these properties in the front matter:

```markdown
---
opengraphimage: images/sharepage.jpg
opengraphtitle: This is my page-level sharing title!
description: This description will be added both to the SEO meta description as well as the share description.
opengraphdescription: If you want your open graph description to be different then your SEO description, use both!
---
```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## License

MIT