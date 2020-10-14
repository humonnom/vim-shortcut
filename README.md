# vim Editor shortcut (linux)   
   
---------------------------------------------------   
## 줄이동   
	맨 뒤로: esc mode + G   
	맨 앞으로: esc mode + gg   
   
---------------------------------------------------   
## how to use esc mode?   
	k ▲   
	j ▼   
	h ◄   
	l ►   
		   
	글자 하나만 바꾸고 싶다면? r   
	단어하나만 바꾸고 싶다면? cw-change word   
	지운다음에 뭐가 바로 쓰고 싶다면?cc-change change   
	한 문장을 지우고 싶다면? dd-del del   
	복사하고 싶다면? yy-y(don't you use)y?   
   
---------------------------------------------------   
## 되돌리기      
   
	작업취소 : esc mode에서 u      
	취소한 작업 복구 : ctrl + r      
   
---------------------------------------------------   
## 추가, 삭제, 검색, 바꾸기   
   
	-선택추가 & 삭제   
	선택추가 : 블록지정 + :norm i[추가하고 싶은 것]      
	  	ex) :norm i//(주석처리)   
	선택삭제 : 블록지정 + :norm [삭제하고 싶은 글자 갯수]x      
  		ex) :norm 2x(주석해제)   
   
		-- visual mode(블록지정) --   
		shift + v : line 전체 블록지정      
		shift + v + 방향키 : 문단 블록지정   
   
	-모든 줄에 추가 & 삭제   
	모든 라인의 앞 부분에 문자 추가	:%norm I[ 넣고 싶은 문자]   
		ex) :%norm I?   
	모든 라인의 뒷 부분에 문자 추가	:%norm A[ 넣고 싶은 문자]   
		ex) :%norm A?   
			모든 라인뒤에 물음표 추가   
	   
		-- 알아두면 편한 i & I & A의 의미 --   
		i : 현재 커서 기준   
		I : 현재 커서가 있는 line 가장 앞부분 기준   
		A : 현재 커서가 있는 line 가장 뒷부분 기준   
		   
	-검색 : esc mode + /[target word]   
		ex) /water   
			"water"가 포함된 모든 단어 검색   
			n을 누르면 다음 단어로 넘어감   
   
	-바꾸기: esc mode + :[범위]/[target word]/[바꿀 단어]/[option]   
		ex) :%s/woter/water/gc   
			%s: 모든 범위에서   
			woter이란 단어를 water로 바꾼다.   
			g: global하게 찾아라(전부 찾아라)   
			c: check하면서 바꾸겠다.(y/n로 선택가능) 
---------------------------------------------------   
## 비쥬얼 블록 모드(Visual block mode)	
   
---------------------------------------------------   
## Cursor는 놔둔채 보이는 화면만 이동하기   
   
	ctrl + y : 위로 더보기 (Screen move up)      
	ctrl + e : 아래 더보기 (Screen move down)    
   
---------------------------------------------------   
## buffers : 버퍼를 사용하면 파일간에 복사 등이 용이함   
   
	Buffers 보기   
	esc mode에서 :buffers   
	file 이름 옆에 적힌 번호로 이동가능함   
	ex) esc mode에서 :b1   
   
	Add buffer   
	esc mode에서e [경로]   
	ex) e ../c_files/target.c   
   
	주의사항 : buffer간에 이동하기 전, 저장먼저 하자   
---------------------------------------------------   
   
