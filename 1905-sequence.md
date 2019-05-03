
# **** 1905-sequence

## *** overview 

- Sequence Types
  + Sequences represent ordered sets of objects indeed by non-negative integers and include strings, lists, and tuples.

## *** logs 


```python
import logging.config
```


```python
logging.config.fileConfig('./logging_debug.conf')
logger = logging.getLogger(__name__)
```


```python
logger.info('------ start...')
```

    [2019/05/03 08:21:27][INFO](1) ------ start...
    

## *** contents 

### ** Operations Common to All Sequence 


```python
s = '012345678'
```


```python
res = s[1]
logger.debug(f's[1] = "{res}"')
```

    [2019/05/03 08:21:27][DEBUG](2) s[1] = "1"
    


```python
res=s[1:5]
logger.debug(f's[1:5] = "{res}"')
```

    [2019/05/03 08:21:27][DEBUG](2) s[1:5] = "1234"
    


```python
res=s[1:9:2]
logger.debug(f's[1:9:2] = "{res}"')
```

    [2019/05/03 08:21:27][DEBUG](2) s[1:9:2] = "1357"
    


```python
res=len(s)
logger.debug(f'len(s) = {res}')
```

    [2019/05/03 08:21:27][DEBUG](2) len(s) = 9
    


```python
s = 'python'
res=max(s)
logger.debug(f'max(s) = "{res}"')
```

    [2019/05/03 08:21:27][DEBUG](3) max(s) = "y"
    


```python
res=min(s)
logger.debug(f'min(s) = "{res}"')
```

    [2019/05/03 08:21:27][DEBUG](2) min(s) = "h"
    


```python
lst=list(s)
lst
```




    ['p', 'y', 't', 'h', 'o', 'n']



// --- end of notebook --- //
