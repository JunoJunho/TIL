# Connecting Virtualenv, Autoenv, pyenv

이번에는 Python의 pyenv와 연동하여 사용가능한 가상환경 virtualenv와 자동으로 가상 환경을 전환해주는 autoenv와의 연동을 해보자.

설치는 다음과 같이

```
$ brew install pyenv-virtualenv
$ echo 'eval "$(pyenv virtualenv-init -)"' >> ~/.bash_profile
$ source ~/.bash_profile
```

위의 쉘 스크립팅은 virtualenv의 설치 이후, virtualenv와 pyenv 설정 값을 bash 프로파일에 넣어주는 작업이다.

사용할 때에는 다음과 같이 사용할 수 있다.

```
$ pyenv virtualenv 3.5.2 virtualenv-3.5.2
# 위와 같이 수행하면 이제 pyenv의 3.5.2 버전을 새롭게 복사해서 가상 환경 virtualenv-3.5.2로 만들 수 있다.
$ pyenv activate virtualenv-3.5.2
# 이렇게 사용 가능하다.
```

그러나 매번 사용할 때마다 활성화 시키고 하는 작업은 매우 귀찮으므로, autoenv를 활용해서 프로젝트 디렉토리를 들어갈 때마다 적용할 수 있다.

```
$ brew install autoenv
$ echo 'source /usr/local/opt/autoenv/activate.sh' >> ~/.bash_profile
$ source ~/.bash_profile
```

예를 들어, env_test라는 프로젝트 디렉토리가 있고 앞서 생성한 virtualenv-3.5.2를 매번 활성화 시키고 싶을 때에는

```
$ touch .env
$ echo "pyenv activate virtualenv-3.5.2" > .env
```

위와 같이 설정이 가능한데, autoenv가 .env 파일이 있는 디렉토리에 접근하면 자동으로 이 가상환경을 활성화 시켜준다.