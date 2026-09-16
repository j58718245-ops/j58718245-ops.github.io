[깃허브 페이지 올리는 순서]

1. github.com 가입 후 오른쪽 위 + → New repository
2. Repository name: 아이디.github.io  (예: thecleancompany.github.io)
   Public 선택 → Create repository
3. "uploading an existing file" 클릭 → 이 폴더 안의 html 파일 전부와
   images 폴더를 통째로 끌어다 놓기 → Commit changes
   (build.py, template.html, README.txt는 안 올려도 됩니다)
4. 1~2분 뒤 https://아이디.github.io/ 에서 지역 목록(index.html) 확인
   지역 페이지 예: https://아이디.github.io/cheonan-unitcooler.html
5. 주소가 확정되면 각 html 상단의 canonical 과 og:image 두 줄에서
   "아이디" 부분을 실제 아이디로 바꿔야 합니다.
   → 메모장 대신 VS Code 같은 편집기에서 "폴더 전체 찾아 바꾸기"로
     "아이디.github.io" → "실제아이디.github.io" 한 번에 바꾸면 됩니다.
6. 네이버 서치어드바이저(searchadvisor.naver.com)와 구글 서치콘솔에
   https://아이디.github.io 등록 → "웹 페이지 수집 요청"으로
   index.html 과 지역 페이지 주소를 제출

[지역 추가·수정]
build.py 안의 REGIONS 목록에 지역을 추가하거나 문구를 고친 뒤
python3 build.py 를 실행하면 전체 페이지가 다시 만들어집니다.
(파이썬이 없으면 지역 목록만 정리해서 보내주시면 제가 만들어 드립니다.)

[파일 이름 규칙]
지역영문-unitcooler.html  예) seosan / dangjin / cheonan / daejeon / sejong
                             jeonju / gunsan / iksan / buan ...
