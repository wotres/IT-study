# Mac 사용
## 단축키
* mac finder(맥 파인더) 에서 상위 폴더 이동 단축키
  * command + 위화살표

## 설정
* nvm 설치
  1. 다운로드
    * $ curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.1/install.sh | bash
  2. 경로 설정 후 설정 추가
    * $ vim ~/.zshrc
      ```
      export NVM_DIR="$HOME/.nvm"
      [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
      [ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion
      ```
  3. 반영
    * $ source ~/.zshrc
  4. 확인
    * $ nvm --version
  
  * 참고 사이트
    * https://github.com/nvm-sh/nvm

* nvm 으로 node 설치
  1. 다운로드 가능 버전 확인
    * $ nvm ls
    * $ nvm ls-remote
  2. 다운로드
    * $ nvm install 20.17.0
  3. 사용
    * $ nvm use 20.17.0
  4. 확인
    * node -v
  * 참고 사이트
    * https://github.com/nvm-sh/nvm
    * https://github.com/nodejs/Release
    * https://nodejs.org/en/download/package-manager


* python 버전 변경
  1. release 현황 확인
    * https://devguide.python.org/versions/
  2. 원하는 버전 설치
    * $ brew install python@3.11 
  3. 설치 경로 확인
    * $ brew --prefix python@3.11
  4. 해당 경로를 바라보게 설정
    * $ alias python='/opt/homebrew/opt/python@3.11/bin/python3.11'
  5. 반영
    * $ source ~/.zshrc
  6. 확인
    * $ python -V

* Python 프로젝트 패키지 의존성 관리 (Pipenv 사용법)
  1. 설치
    * $ pip install pipenv
  2. 원하는 패키지이름
    * $ pip install [패키지명]
    * 특정 버전의 패키지 설치
      $ pip install 패키지명===2.25.0
  3. 설치된 패키지 확인
    * Pipfile or Pipfile.lock 확인
    * $ pipenv graph



