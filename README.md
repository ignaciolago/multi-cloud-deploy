# helm-tutorial
helm Chart examples and tutorial resources

This is an example charts repository.

### How It Works

I set up GitHub Pages to point to the `docs` folder. From there, I can
create and publish docs like this:

# library-demo

```
$ cd library
$ helm package library-chart -d ./docs 
$ helm repo index ./docs
$ cd ..
```

# parent-demo
```
$ cd parent
$ helm dependency update nginx-chart
$ helm package nginx-chart -d ./docs
$ helm repo index ./docs
$ cd ..
```