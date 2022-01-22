## 명령 모드

- `ESC` 누른 상태가 명령 모드

- `:set nu` : 라인 출력

- `i` : insert 모드로 변경

- `:{line number}` : 해당 라인으로 이동

- `:wq` : 저장하고 종료(`ZZ`도 동일)

- `:q!` : 강제 종료

- `w, b` : 단어 단위 이동

- `dd` : 줄 삭제

- `v` : 블럭 지정

- `?{검색할 단어}` : 윗부분에서 검색

- `/{검색할 단어}` : 아랫부분에서 검색

- `^, $` : 라인 처음, 끝으로 이동

- `o, O` : 커서 밑, 위에 빈 행 추가하며 입력

- `r` : 현재 커서에 있는 글자 바꾸기

- `s` : 현재 커서 글자 바꾸고 입력모드

- `yy`: 라인 복사

  - `p` : 라인 복사 후 붙여넣기

- `H, L` : 현재 스크린에서 출력된 첫 라인, 마지막 라인으로 이동

- `control + v` : 컬럼 블록

- `shift + v` : 줄 단위 블록

- `G` : 마지막 행으로 가기

- ```plaintext
  %s/{Old 단어}/{New 단어}/gc
  ```

   

  : Old 단어를 New 단어로 변경(바꾸기 전에 물어봄)

  - `/g`는 글로벌 옵션
  - `/c`는 컨펌 옵션

- `u` : 이전으로 되돌리기(undo)

- `control + r` : 되돌리기한 것을 다시 실행(redo)

- ```plaintext
  :v/관심패턴/d
  ```

   

  : 관심 패턴 라인만 남겨서 볼 경우

  - 로그 분석시 사용
  - `u` 눌러서 복구

## 실행시

- `vi -d A파일 B파일` : 다른 부분들 하이라이트







출처: https://zzsza.github.io/development/2018/07/20/vim-tips/
