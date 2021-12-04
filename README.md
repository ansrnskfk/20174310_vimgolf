# 20174310_vimgolfㅁ

> 오픈소스SW개론 과제#2 vimgolf 20174310 이경근

 ---

**1. Add quotes to ansible playbook**

![vimgolf_1](https://user-images.githubusercontent.com/38202602/144698504-db5f85c5-c71b-429f-bb40-c29e0a23d2c5.gif)

![시도1-1](https://user-images.githubusercontent.com/38202602/144698613-fde7d753-cd9e-4a3f-8424-80a8a4eccad1.JPG)

`G`: 파일의 마지막 줄로 이동.

`W`: 띄어쓰기 전까지 한 단어로 취급, 단어의 오른쪽 끝으로 이동.

`I`: 입력모드.

`"<End>"`: 커서가 위치한 곳과 줄의 끝에 " 입력.

`<Esc>`: 일반모드.

---

**2. simple replacements**

![vimgolf_2](https://user-images.githubusercontent.com/38202602/144698942-1856d8f5-76ae-4052-b726-ea482b805cc4.gif)

![시도2-1](https://user-images.githubusercontent.com/38202602/144699044-0825b647-d2ac-4183-8bda-d78bea68b612.JPG)

`:%s/`: 파일 전체에서

`sublime\|emacs/vim/`: sublime과 emacs를 vim으로 치환

---

**3. Satisfy the go linter**

![vimgolf_3](https://user-images.githubusercontent.com/38202602/144699638-dfa8f3aa-39e0-4200-a42a-a0ef676e2a73.gif)

![시도3-4](https://user-images.githubusercontent.com/38202602/144699627-41df5b0a-f189-46a2-bae1-2ae9baff89ed.JPG)

`:4`: 4번째 줄로 이동.

`yw`: 단어 복사.

`O// TODO`: 바로 윗줄에서 입력모드 진입, // TODO 입력.

`b`: 한 단어 뒤로 이동.

`P`: 현재 위치에 붙여넣기.

`yy`: 줄 복사

`<Down>pw`: 아래줄로 이동 후 붙여넣고 한 단어 앞으로 이동.

`R`: replace 입력모드. (윈도우 키보드 ins키와 유사)

+ 그 밖의 시도들

![시도3-3](https://user-images.githubusercontent.com/38202602/144699939-8a5249fe-6ba7-4ba8-a19d-979e25e86556.JPG)
![시도3-1](https://user-images.githubusercontent.com/38202602/144699940-50764003-3876-4bf0-929e-6d97ff2a86c5.JPG)
![시도3-2](https://user-images.githubusercontent.com/38202602/144699941-59f7bffd-1864-4bc7-85cc-a1db069cae00.JPG)

---

**4. Plotting some variables in python**

![vimgolf_4](https://user-images.githubusercontent.com/38202602/144699951-862cf289-45bb-488f-9f06-9c4c76706ac3.gif)

![시도4-1](https://user-images.githubusercontent.com/38202602/144700509-53a31085-2e3f-4c12-ab24-09cec5b4b8cd.JPG)

`:%s/y1/abs(y1)`: y1을 abs(y1)으로 치환.

`<C-A>`: (CTRL+a) 숫자를 1 증가 시킨다.

`fy`: 앞으로 탐색하면서 y를 찾고, 커서를 이동시킨다.

---

**5. Python dataclasses**

![vimgolf_5](https://user-images.githubusercontent.com/38202602/144700678-cbbabc0c-6ebf-4b03-af9f-827c9fa6bd71.gif)

![시도5-4](https://user-images.githubusercontent.com/38202602/144700682-3b9e2cef-af82-40ec-965e-a5fd2bdca444.JPG)

`4<CR>`: 4줄 밑으로 이동

`qa`: 매크로 기록을 시작하고 그 내용을 a에 저장한다.

`yw`: 단어 복사.

`10G$Pa,`: 10G% - 10번째 줄로 이동 하고 줄의 마지막으로 이동. P - 그 후 붙여넣기. a, - 다음칸에서 입력모드 진입 후 ',' 입력

`<Esc>q`: 일반모드에서 다시 q를 누르면 매크로 기록 종료, 저장.

`@a`: a에 저장된 매크로 실행

`@@`: 직전에 실행된 매크로 실행

`x` : 커서 다음칸에 있는 문자 삭제

+ 그 밖의 시도들

![시도5-1](https://user-images.githubusercontent.com/38202602/144700865-03df2958-dc4c-457f-9b74-c20fb3ad6e97.JPG)
![시도5-2](https://user-images.githubusercontent.com/38202602/144700868-015e0f68-a743-4e9a-aff1-939b4755be47.JPG)
![시도5-3](https://user-images.githubusercontent.com/38202602/144700869-fb2669e3-c478-43f5-afac-8b4234f63174.JPG)


