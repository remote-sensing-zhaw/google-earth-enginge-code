

## General

- Stance Maples has an awesome introduction to GEE on [youtube](https://youtu.be/oAElakLgCdA).
- Didactics: 
  - When walking through the code, try to involve the students in the thought processes that it might take to come up with the correct solution.
  - The classification example is ~~outdated, especially since the training data needs to be uploaded. There is usually not enough time to do this anyway.~~ a standalone script that I presented in different lecture

## Git Stuff

This repo has two origins:

```
$ git remote -v

origin  https://earthengine.googlesource.com/users/rata/zhaw-remote-sensing (fetch)
origin  https://earthengine.googlesource.com/users/rata/zhaw-remote-sensing (push)
upstream        https://github.com/remote-sensing-zhaw/google-earth-enginge-code.git (fetch)
upstream        https://github.com/remote-sensing-zhaw/google-earth-enginge-code.git (push)
``` 

Both origins should be in sync, for each origin there is one branch named master.

To push to github, do as you normally push. To push to earthengine, try pushing, then click on the link provided in the error message, then copy the command provided on the website after authentication and paste it into the terminal. Push again and it will work.

```
git push origin master
git push upstream master
```



