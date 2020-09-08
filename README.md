# vim Editor shortcut (linux)

## 되돌리기   

작업취소 : esc mode에서 u
취소한 작업 복구 : ctrl + r   

## Visual mode   

shift + v : line 전체 블록지정   
shift + v + 방향키 : 문단 블록지정

주석처리 : 블록지정 + :norm i[추가하고 싶은 것]   
  ex) :norm i//
주석삭제 : 블록지정 + :norm [삭제하고 싶은 글자 갯수]x   
  ex) :norm 2x

## Cursor는 놔둔채 보이는 화면만 이동하기

ctrl + y : 위로 더보기 (Screen move up)   
ctrl + e : 아래 더보기 (Screen move down)   
