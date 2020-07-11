# BashRC

- This is only partial contents of the bashrc.
- Use this in addition to the default bashrc.

## Location : 
- ~/.bashrc

## Contents

```
# Ciarans Bashrc

# Tested in Ubuntu 18.xx, 


# Use this in Ubuntu etc, mac has ZSH by default as it's editor so use ohmyzsh

[Git branches in terminal](https://gist.github.com/joseluisq/1e96c54fa4e1e5647940)


########
# Custom
#######


dockerjoin(){
    sudo docker exec -it $1 /bin/bash
}


git-undo-index(){
    # $1 Path to file
    git checkout HEAD --$1
}

git-reset(){
    git checkout -- $1
}

#For when I forget caps lock is on
alias CD='cd'
alias LS='ls'
```