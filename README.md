# clone-all-github-repo
script to clone all github repo using token

```
https://api.github.com/user/repos?per_page=100 | grep ssh_url | cut -d ':' -f 2-3|tr -d '",'`; do git clone $i; done
```
