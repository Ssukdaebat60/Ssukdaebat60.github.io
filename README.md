My Git Blog
========================================
----------------------------------------------------------
1)  github.io
 >Git에서 username.github.io의 형식으로 repository를 생성한다.   

그러면 인터넷 주소창에 username.github.io를 입력하면 블로그로 이동할 수 있게 된다.   
이는 복잡한 과정없이 블로그를 개설할 수 있게 해준다.

- - -
2)  Remote to Local
> ```git clone username.github.io```  

Git의 원격 repo를 로컬에 복사하여 연결한다.

- - -
3) Jekyll   
>
```
gem install bundler jekyll   
jekyll new myblog   
cd myblog   
bundle exec jekyll serve
```
정적 웹사이트를 쉽게 만들어 주는 Jekyll을 이용한다.   
위와 같이 Jekyll을 다운 받고 실행 시키면 웹사이트를 쉽게 관리할 수 있다.

 - - -
4) Theme
> 원하는 테마를 git에서 찾아 로컬의 repo에 덮어쓴다. 
 
모든 설정이 다운 받은 테마에 맞춰진다.  
**_post 파일에 미리 쓴 문서가 있다면 _post는 덮어쓰지 않는다.**

- - -
5) configuration
> _config.yml에서 url와 baseurl이 설정되어 있다면  본인 블로그의 주소로 넣어야 테마가 제대로 적용된다.  
(공란으로 만들어도 되는 경우가 있음)

블로그 제목이나 기타 다른 정보들도 본인의 블로그에 맞게 수정한다.
- - -
6) post
> _post 파일에 yyyy-mm-dd-title.md 형식으로 마크다운 파일을 만들고 내용을 작성한다.  

>
```
---
layout : post
title : FirstPost
 .
 .
 .
---
```
다음과 같은 파일의 헤더 부분을 추가해서 포스트의 정보를 설정할 수 있다.

- - -
7) Markdown
> 포스트는 마크다운을 이용해서 작성할 수 있다.  

[사용법](https://gist.github.com/ihoneymon/652be052a0727ad59601)

- - -
8) Add Comments
> Utterances를 이용해서 댓글을 추가한다.[사용법](https://velog.io/@outstandingboy/Github-%EB%B8%94%EB%A1%9C%EA%B7%B8%EC%97%90-%EB%8C%93%EA%B8%80-%EA%B8%B0%EB%8A%A5-%EC%B6%94%EA%B0%80%ED%95%98%EA%B8%B0-ft.-Utterances)  
그리고 각 포스트의 헤더 부분에 comments : true를 추가한다.
```
---
layout : post
title : FirstPost
comments : true
---
```

성공적으로 댓글창이 생성된다.  
![댓글창](/comments.png)  
그러나 다크모드는 적용되지 않는다.  
(블로그를 다크모드로 바꿔도 댓글창은 그대로 하얀 바탕이다.)
