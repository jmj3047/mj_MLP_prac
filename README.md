# mj_MLP_prac

### cloning: error for file path is too long
```bash

jmj30@LAPTOP-D1EUIRLS MINGW64 ~/Desktop
$ git clone https://github.com/jmj3047/mj_MLP_prac.git
Cloning into 'mj_MLP_prac'...
remote: Enumerating objects: 540, done.
remote: Counting objects: 100% (212/212), done.
remote: Compressing objects: 100% (176/176), done.
remote: Total 540 (delta 19), reused 207 (delta 17), pack-reused 328
Receiving objects: 100% (540/540), 132.09 MiB | 3.23 MiB/s, done.
Resolving deltas: 100% (42/42), done.
error: invalid path 'runs/2022-04-28 15:05:31.008493-MLP/events.out.tfevents.1651125932.langtech.16343.0'
fatal: unable to checkout working tree
warning: Clone succeeded, but checkout failed.
You can inspect what was checked out with 'git status'
and retry with 'git restore --source=HEAD :/'


jmj30@LAPTOP-D1EUIRLS MINGW64 ~/Desktop
$ ls
desktop.ini  mj_MLP_prac/ 

jmj30@LAPTOP-D1EUIRLS MINGW64 ~/Desktop
$ cd mj_MLP_prac/

jmj30@LAPTOP-D1EUIRLS MINGW64 ~/Desktop/mj_MLP_prac (master)
$ git restore --source=HEAD :/
error: invalid path 'runs/2022-04-28 15:05:31.008493-MLP/events.out.tfevents.1651125932.langtech.16343.0'
...


jmj30@LAPTOP-D1EUIRLS MINGW64 ~/Desktop/mj_MLP_prac (master)
$ git config --system core.longpaths true

jmj30@LAPTOP-D1EUIRLS MINGW64 ~/Desktop/mj_MLP_prac (master)
$ ls
'MLP+Optimizers(scheduler).ipynb'                          data/
'MLP+basic regularizers(dropout + early stopping).ipynb'   data_utils.py
 MLP.ipynb                                                 logs/
 README.md                                                 requirements.txt
 __init__.py                                               wandb/
 __pycache__/

```