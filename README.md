<h1><img src="https://em-content.zobj.net/thumbs/160/microsoft/319/star_2b50.png" height="30px"/> pnpm package manager for window</h1>

![PNPM](https://img.shields.io/badge/pnpm-%234a4a4a.svg?style=for-the-badge&logo=pnpm&logoColor=f69220)

<h3> Now, explain about pnpm </h3>

* pnpm 패키지 매니저
1. pnpm은 모든 프로젝트에서 패키지를 공유할 수 있는 단일 캐시를 사용하기 때문에 디스크 공간을 절약할 수 있다.
2. pnpm은 프로젝트마다 패키지를 복사하지 않고 하드 링크를 사용하여 공유한다.
3. pnpm은 yarn과 동일하게 병렬로 패키지를 설치할 수 있어서 설치 시간을 단축할 수 있다.
4. 큰 프로젝트에서 유리하다.
5. 패키지가 로컬에 이미 설치되어 있는 경우 다시 다운로드하지 않고 해당 패키지를 재사용할 수 있다.

* pnpm 설치 및 세팅, 사용법
1. nodejs 설치 (https://nodejs.org/ko)
2. cmd 활성화
3. node -v로 node 설치 여부(버전 확인)
4. cmd 창에서 npm install -g pnpm 명령어로 pnpm 로컬 전역에 설치
5. pnpm -v로 버전 확인
4. vscode에서 터미널 활성화한 후 다음 명령어로 해당 폴더에 package.json파일 생성 : $  pnpm init
5. 다음 명령어로 pnpm.lock 파일과 모듈 설치 : $ pnpm install
-> 만약에 package.json 파일을 가지고 있더라면, package.json안에 있던 패키지들이 자동으로 설치
6. 끝

* pnpm 명령어로 pakage.json 파일 사용법
1. pnpm add 패키지명 : 해당 패키지 설치(추가)
2. pnpm update : 설치된 패키지들을 업데이트
3. pnpm remove 패키지명 : 설치된 패키지들을 삭제
4. pnpm dedupe : pnpm 중복된 패키지들 정리
5. pnpm root : node_modules 설치 경로
6. pnpm test or start : package.json의 script 부분에 아래와 같이 입력하여 간단하게 실행가능. 하지만 입력하지 않았다면 node server.js가 실행
    "scripts": {
        "test": "echo \"Error: no test specified\" && exit 1",
        "start": "node index.js"
    },
7. pnpm search : 패키지 검색
8. pnpm run : package.json 파일의 scripts 항목에서 정의된 스크립트를 실행
