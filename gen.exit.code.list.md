```
grep -hr exit\  . | sed 's/echo\ //g' | sed 's/exit\ //g' | awk '{ print  }' | sort | uniq
```
