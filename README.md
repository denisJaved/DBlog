### Hi, there!
**DBlog** is static files based blogging system. With DBlog you can make our own blog very easly and you don't need any fancy hostings becouse you can use [github pages](https://docs.github.com/en/pages) for it!

## Getting started with github pages
```
This tutorial is for DBlog V1
```

To get started with DBlog you need to create repo with github pages. [tutorial here](https://docs.github.com/en/pages/quickstart)

You can skip [`_config`](https://docs.github.com/en/pages/quickstart#changing-the-title-and-description) part. Title and description controlled by DBlog.

### Creating page
To create page you want to create json file named how you want (for example: `how-to-create-dblog-page.json`. PS: file name has NO effect to actuall dblog page). 

Then you need to fill it with code below.
```json
{
  "title":"blog page title here",
  "type":"content type here",
  "contents":"content of page here"
}
```
title key should be filled with title of your blog post

type key contains information about type of content you wanna post

contents field used for contents of your post like if type is html, contents can be `<p> I'm <b>blod</b></p>` or `First line \n SecondOne` for text type (this is just examples)

## Current types:
| Type key value | Description                             |
|----------------|-----------------------------------------|
| text           | plain text (line breakes supported)     |
| html           | just html useed by browsers             |

### And now you done!
You can visit `https://denisjaved.github.io/blog/v1/page?source=github::<your github username goes here>&path=<path goes here>`

```
        yourusername.github.io/blog/yourjsonfile.json 
You can find path              ↑ ↑ ↑ ↑ ↑ ↑ HERE ↑ ↑ ↑ 
```
In this example it will be `blog::yourjsonfile`, you can get it by removing `.json` and replacing all `/` by `::`
