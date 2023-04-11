# helm library and parent 
this is a library and parent helm charts 
ths sould be stay in sepaate repos but to simplfy we use the same  

### How It Works

Here setup GitHub Pages to point to the `docs` folder. From there, then you can
create and publish docs with version of bot components 
with dthe folling commands , be crate the index and respective docs to be plushied in github pages to be user later bor umbrella in gitops components: 


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
