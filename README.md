# ReactBlog blog-engine

A jekyll style blog react component set and scripts for any react app.

Configure you blog in `package.json`.

Create markdown files with grey matter using the cli.

For example, `yarn newpost -- --title='Awesome Idea' --description='details of awesome idea'`.

Write markdown files in the folders of your choosing.

Install a default blog route in your react router setup.  Will interpret slugs and find the right post.

Or customize your blog with simple components `<BlogPost />`, `<BlogIndexPage />`, or `<BlogApp />`

----

# Install

* run `yarn add reactblog`

Add `reactBlog` specific props to `package.json`

```json
{
  "name": "Your Project - imagine more properties in this file"
  "reactBlog": {
    "publicFolder": "/public",
    "markdownFolderInPublicFolder": "/blog-markdown",
    "postFolder": "/blog-pages"
  }
}
```

----

## Components

`<BlogPost syntaxStyle-{'default'}>`


`<BlogIndexPage />`


`<BlogApp />`

Used in a route to create a full app that renders with a header, footer, starts with the index page, and clicks to the blog post page.