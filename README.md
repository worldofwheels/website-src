### World of Wheels Website

#### Publishing Process:

1. Make changes as necessary, ensure they look right by testing [locally](http://localhost:1313) : 

```bash
$ hugo server -D
```

2. Remove the public directory and force a rebuild

```bash
$ rm -rf public/
$ hugo
```

3. Commit and push this repository, then commit and push the `public` submodule:

```bash
$ git add -A . && git commit -m "made some changes" && git push -u origin master
$ cd public/
$ git add -A . && git commit -m "made some changes" && git push -u origin master
```