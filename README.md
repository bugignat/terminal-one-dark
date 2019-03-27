# Terminal One Dark Theme

```sh
source /usr/local/etc/bash_completion.d/git-completion.bash

parse_git_branch() {
  git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/ (\1)/'
}

export PS1="\[\e[32m\]\w\[\e[97m\]\[\e[2m\]\$(parse_git_branch)\n❯ \[\e[0m\]"
```
