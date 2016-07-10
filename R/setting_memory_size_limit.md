# Memory size limit setting

Window 시스템에서 R을 사용할 때 가끔씩, 너무 많은 데이터를 하나의 변수에 담으려고 하다보면, 자바 Garbage Collection error가 발생함. 이런경우, 하나의 대안으로는 한번에 들 수 있는 메모리 량을 증가시키는 방법이 있음

```
memory.limit(size=250000) # Set limit as 250000 bytes
```
