## how to serve

`jekyll serve --watch `

## how to deploy

you need to be on branch "source".
Only there you can edit the source, e.g. `_pages/media.md`

THEN: if on wrong branch, i.e. if on branch "gh-pages", do:
- git checkout source
- git reset --hard
- git clean -fd

then commit new source and git push origin source.

Then finally:
`JEKYLL_GITHUB_TOKEN= <token> PAGES_REPO_NWO=mueller91/mueller91.github.io bin/deploy_old`

get token from ~/.ssh/git_code.txt



