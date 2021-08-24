# Issue with jekyll-github-metadata

There is an [issue](https://github.com/jekyll/github-metadata/issues/213) with the `github_edit_link` produced by [jekyll-github-metadata](https://github.com/jekyll/github-metadata) for paginated pages.

Actually, the issue is from [jekyll-paginate](https://github.com/jekyll/jekyll-paginate), because `page.path` contains the paginated path and that is used by the edit link, but that repo is no longer maintained.

## Demo

```
bundle install
bundle exec jekyll serve
```

Then open https://127.0.0.1/github-edit-link-issue/page/2/
