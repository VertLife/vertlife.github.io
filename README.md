# VertLife  
The VertLife website. This is a jekyll site that uses kramdown flavored markdown and Bootstrap css. 


To run locally in a docker environment run: 

```
docker run --rm \
  --volume="$PWD:/srv/jekyll" \
  -p 4000:4000 \
  jekyll/jekyll \
  jekyll serve --host 0.0.0.0
```