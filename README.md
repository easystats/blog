# blog
:mega: The collaborative [blog](https://easystats.github.io/blog/).



## How to publish a post

1. Fork this repo to your account
2. Duplicate one of the Rmarkdown file of a blog post already written in `/content/posts`
3. Rename this new file
4. Open `blog.Rproj` in R and then open your new file
5. Edit your new blogpost (the `Rmd` file) as you want
6. Run `blogdown::serve_site()` to see it locally
7. Run `blogdown::build_site()`
8. Once  you're satisfied, close R and R studio.
9. **Important steps**:
  - Go to `/docs/categories/r` and open `index.xml` with a notepad. Search for all the `/blog/blog/` strings and replace by `https://easystats.github.io/blog/` if you see that the URLs is relative or just by `blog` otherwise. `blogdown::build_site()` also changes older files (older blog posts), and create non-working URLs containing `/blog/blog/` again - make sure these are fixed to the full website URL.
  - Make sure all images in your post have _absolute paths_, and not relative URLs, for example: `https://easystats.github.io/blog/posts/see_presentation_files/figure-html/unnamed-chunk-3-1.png`.
10. Publish this new content on a new github branch named `post-uniquepostname`
11. Do a PR for this branch to be merged into master
