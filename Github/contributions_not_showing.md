## github 잔디 안 심어지는 현상

![](https://www.github.com/ingyeomnote/TIL)

오늘도 평소처럼 main 브랜치에 push를 했는데 github에 잔디(github contributions)가 심어지지 않았다. 이유는 간단했는데, github 계정에 등록된 이메일과 commit해서 push를 진행하는 local 환경의 이메일 설정이 다르기 때문이었다.

![](https://github.com/ingyeomnote/TIL/blob/main/Github/images/contributions.PNG?raw=true)



### github 등록 이메일 확인

github에 등록된 이메일을 확인하려면 계정[Settings -> Emails] 메뉴로 들어가면 된다. 

### git local 환경의 이메일 확인

작업중인 폴더에서 cmd 또는 git.bash를 열고 아래 명령어를 치면

```
git config user.email
```

user.email 값을 확인할 수 있다. 만약, 여기서 email 값이 다르다면 작업중인 폴더에서 commit을 하더라도 잔디가 심어지지 않는다.

![](https://github.com/ingyeomnote/TIL/blob/main/Github/images/checking_user_email.PNG?raw=true)


git config user.email로 확인했을 때 등록된 이메일은 kng03318@gmail.com이었다. 이는 github에 등록된 이메일이랑 달랐기 때문에 잔디가 심어지지 않았다.

### git local 환경의 이메일 변경

작업중인 폴더에서 cmd 또는 git.bash를 열고 아래 명령어를 치면

```
git config user.email "변경하고 싶은 주소"
```

local 환경의 email 값을 변경할 수 있다.

![](https://github.com/ingyeomnote/TIL/blob/main/Github/images/changing_user_email.PNG?raw=true)

이제 다시 push를 진행하면 아래처럼 잔디가 잘 심어지는 것을 확인할 수 있다.

![](https://github.com/ingyeomnote/TIL/blob/main/Github/images/contributions02.PNG?raw=true)


