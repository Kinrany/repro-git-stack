Current tree:

```
* main
| * branch2
| * branch1
|/
* main2
```

Do this:

```
git switch main2
git stack --rebase --onto main
```

Expected result:

```
* branch2
* branch1
* main, main2
*
```

Found:

```
* branch2
* branch1
* main
* main2
```

---

Reproducing a bug in git-stack
