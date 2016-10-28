# Trouble Shooting at installing 3.5.2 on OS X

OS X 환경에서 3.5.2 버전을 설치하다 보면 sqlite3를 찾지 못했다면서 에러가 발생하는 경우가 있습니다.

이 경우는 아래와 같이 xcode의 커맨드라인 툴을 설치해주면 됩니다.

```
$ xcode-select install
```

그러면 알아서 xcode에 필요한 툴을 설치하면서 겸사겸사 디펜던시도 해결해 주는 것 같네요