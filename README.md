# Nebuloid Articles
This repository contains the article files for the Nebuloid Blog.
Feel free to peruse it as you will!
However, be sure to check out the main website, [nebuloid.dev](https://nebuloid.dev).
The viewing experience is much better there!
📰😁👍

Alternatively, you may be interested in the other repositories in Project Nebuloid.
If that is the case, you can browse the other repositories at [github.com/nebuloid-blog](https://github.com/nebuloid-blog).

## Contributing
You can suggest additions or modifications to articles in my blog.
Even a small spelling error fix or grammar fix is very much appreciated.

You can [create an issue](https://github.com/nebuloid-blog/articles/issues/new) to point out an error or make a suggestion.
Thanks for your help!

## Unified
![](https://raw.githubusercontent.com/unifiedjs/unified/93862e5/logo.svg?sanitize=true)

All of the articles contained in this repo are written in HTML fragments.
While they could have instead been written in markdown, I found it easier to work with HTML.

At the end of the day, the actual format doesn't matter, because [**UnifiedJS**](https://unifiedjs.com/) can convert it all into a UAST (Unified Abstract Syntax Tree), regardless of the format.
Unified can work with [Markdown](https://remark.js.org/), [HTML](https://github.com/rehypejs/rehype), and more.
Once you convert the content with Unified, its an easy job to tweak, sanitize, and output to JSX (or whatever else you want to do).

## Front Matter
Front matter is a way to organize metadata in content like markdown and HTML fragments.
It acts like an informal document head of sorts, and is particularly useful for its interaction with the API.

I use a [TOML-based](https://toml.io/en/) frontmatter (denoted by `~~~`) in this repository, to maintain metadata for each article.

### Standardized Keys
The following keys exist for articles in this repo:

| Name                | Required                | Unique                  | Immutable               | Type    |
| ------------------- | :---------------------: | :---------------------: | :---------------------: | ------- |
| id <sup>[1]</sup>   | :ballot_box_with_check: | :ballot_box_with_check: | :ballot_box_with_check: | integer |
| slug <sup>[2]</sup> | :ballot_box_with_check: | :ballot_box_with_check: | :ballot_box_with_check: | string  |
| title               | :ballot_box_with_check: |                         |                         | string  |
| description         |                         |                         |                         | string  |

<small>
	<sup>[1]</sup> This is immutable; the database relies upon IDs for things like comments and permalinks.<br />
	<sup>[2]</sup> This slug shall only contain lowercase alphanumeric characters "a-z" "0-9", and the dash character "-".
</small>
