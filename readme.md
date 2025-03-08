## Git branching example

```
git commit -a -m "m1"
git commit -a -m "m2"
git commit -a -m "m3"
git log --graph --oneline --all --decorate 
```

![0.png](0.png)


```
git branch try_e
git switch try_e
git commit -a -m "e1"
git commit -a -m "e2"
git log --graph --oneline --all --decorate 
```

![1.png](1.png)


```
git switch main
git branch try_f
git switch try_f
git commit -a -m "f1"
git log --graph --oneline --all --decorate 
```

![2.png](2.png)


```
git switch main
git merge try_e
git commit -a -m "m4"
git log --graph --oneline --all --decorate 
```

![3.png](3.png)


```
git commit -a -m "m5"
git log --graph --oneline --all --decorate 
```

![4.png](4.png)


```
git switch try_e
git commit -a -m "e3"
git log --graph --oneline --all --decorate 
```

![5.png](5.png)


```
git switch main
git push
git log --graph --oneline --all --decorate 
```

![6.png](6.png)


```
git switch try_f
git push --set-upstream origin try_f
git log --graph --oneline --all --decorate 
```

![7.png](7.png)


```
git switch try_e
git push --set-upstream origin try_e
git log --graph --oneline --all --decorate 
```

![8.png](8.png)

