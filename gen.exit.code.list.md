From http://tldp.org/LDP/abs/html/exitcodes.html "exit codes 1 - 2, 126 - 165, and 255 [1] have special meanings, and should therefore be avoided for user-specified exit parameters."

```
grep -hr exit\  ~/buildAPKs/scripts/bash/ | sed 's/echo\ //g' | sed 's/exit\ //g' | awk '{ print  }' | sort | uniq
```
Further reading https://unix.stackexchange.com/questions/242111/using-reserved-codes-for-exit-status-of-shell-scripts 
