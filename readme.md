github error 해결법. Authentication failed for _ use a personal access token instead
1. github를 사용하다가 보면 2021년 8월 이후로 git pull을 하려 할 때 아래와 같은 에러가 발생할 수 있다. 
2. 이는 8월부터 id/password 방법이 아닌 token을 이용하여 로그인을 수행하기 때문이다. 
3. 사실 회사나 다른 컴퓨터에서 git id와 password를 조회할 수 있어 토큰 방식이 더 안전한 것 같다. 
4. 아래와 같은 순서로 처리하면 된다. 


1. 깃허브에 접속하여 로그인 한다. https://github.com
2. 우측상단의 정보에서 setting 정보 클릭
3. setting 페이지에서 좌측아래 developer setting click
4. Personal access tokens를 클릭 후 Generate new token 클릭
5. Note 에는 원하는 사용처를 입력하고 expiration에 사용을 원하는 기간 입력되 repo 클릭 후 제일 아래 Generate token 클릭
6. 토큰이 생성되면 반드시 복사(단 한번만 보여짐)
7. 로컬 컴퓨터의 깃에 등록
   git config --global user.name 'id'
   git config --global user.password 'token'

8 additional
