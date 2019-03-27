# Terminal One Dark Theme

```sh
source /usr/local/etc/bash_completion.d/git-completion.bash

parse_git_branch() {
  git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/ (\1)/'
}

export PS1="\[\e[90m\]\w\[\e[95m\]\$(parse_git_branch)\n\[\e[34m\]❯ \[\e[0m\]"
```
