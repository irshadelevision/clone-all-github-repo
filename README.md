# clone-all-github-repo
script to clone all github repo using token

```
for i in `curl -H "Authorization: token [[TOKEN]]" https://api.github.com/user/repos?per_page=100 | grep ssh_url | cut -d ':' -f 2-3|tr -d '",'`; do git clone $i; done
```

[Stack Overflow](https://stackoverflow.com/questions/46725688/how-to-clone-all-repos-including-private-repos-from-github)
