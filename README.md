# curlables.ivstiv.dev

Every so often I happen to stumble upon one of these rare gems on the internet, so I got curious if there is a list of them. Unfortunately, I couldn't find any just by searching, so I started writing them down in notes whenever I find a new one. So I figured to put all of my notes together and make a simple website to save what I have found so far. Do not hesitate to contribute if you know any more web apps that fit this category.

## Setup
You will need [ssg](https://www.romanzolotarev.com/ssg.html) and [lowdown](https://kristaps.bsd.lv/lowdown) in order
to compile the markdown from the "src" folder into a "dst" folder to html. lowdown is a widely available tool that is probably available in your repos, if not just compile it from source it takes less than a minute. ssg is already in the repo in the "bin" directory.

If you want to add a new page just create the markdown file in src according to [this](https://github.com/Ivstiv/curlables/blob/master/src/example-article.md) example and create a PR. 

Compile the project:

```
rm -rf dst && mkdir dst && bin/ssg5 src dst 'Curlable Web Apps' 'https://curlables.ivstiv.dev'
```

## Links
- For more advanced usage consult the [ssg's manual](https://www.romanzolotarev.com/ssg.html).
- [Markdown Syntax Guide](https://www.markdownguide.org/basic-syntax)