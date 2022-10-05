## Group static website template

To make it easier for groups to post information about their activities, we used [HUGO](https://gohugo.io/) as the article platform tool to statically generate blog posts and eventually use GitHub Pages to render the pages, providing a separate page for groups to display the information they need to post. Therefore, you only need to follow the normal way of using HUGO for the whole process.

If you don't have HUGO installed, you can get the HUGO version for your device from the [Release page of the official HUGO GitHub repository](https://github.com/gohugoio/hugo/releases) and place it in the PATH for invocation.

Once the installation is ready, the general common commands are as follows (executed in the root directory of this source code repository).

```
$ hugo server # Start a local server and preview the site content in its current state
$ hugo new posts/my-post.md # Create a new article for editing
$ hugo server -D # Enable local server and be able to preview articles with draft status (`draft: true`)
$ hugo -D # Generate a static page (if required), the generated file will be located in the public directory
```

When creating a post, create it in the format `<category>/<filename>. <format>`, in the example given above, the category is posts, the filename is my-post, and the format is md (markdown). After creating a post, some meta information of the post will be marked with [YAML front-matter](https://gohugo.io/content-management/front-matter/) by default, please note that posts in draft state will not be displayed eventually.

To get HUGO, please refer to the [official documentation for installation](https://gohugo.io/getting-started/installing).

## Suggestions for article content guidance

You can write blog posts to share articles in this blog according to your group's needs, below are guidelines related to the content of the article.

When posting your article, it is recommended to use tags to mark the topics related to your article to make it easier for readers to access your article. For example `tags: ["Results Announcement"]` or `tags: ["Guideline Document", "CMake"]`.

Since in most cases each article represents only your own personal opinion, it is also highly recommended to include author information in the meta information of the article, e.g. `authors: ["Zhang San"]` (multiple people are allowed).

## Improve this template project

This template project uses the [geekblog](https://themes.gohugo.io/hugo-geekblog/) theme (based on `v0.5.3`, with changes), but it is not necessarily complete to meet the needs of each group, if you have any suggestions, you can discuss and modify or provide a more suitable theme.
