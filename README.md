# blog
:mega: The collaborative [blog](https://easystats.github.io/blog/).



## How to publish a post

1. Fork this repo to your account
2. Duplicate one of the Rmarkdown file of a blog post already written in `/content/posts`
3. Rename this new file
4. Open `blog.Rproj` in R and then open your new file
5. Edit your new blogpost (the `Rmd` file) as you want
6. Run `blogdown::serve_site()` to see it locally
6. Run `blogdown::build_site()`
7. Publish this new content on a new github branch named `post-uniquepostname`
8. Do a PR for this branch to be merged into master