[uzinnnnnnn.github.io](https://sinji2102.github.io/)
***
소프트웨어학부 20223059 김유진

![mainpage](assets/img/favicon.png)

## 0. 설치한 것
##### 1. Ruby
`sudo apt install ruby-full`
 [참조 사이트](https://ubunlog.com/ko/ruby-diferentes-formas-de-instalarlo-en-ubuntu-20-04/)
##### 2. jekyll & Bundler
`gem install jekyll bundler`
Jekyll이 올바르게 설치되었는지 확인  
`jekyll -v`
##### 3. git
`sudo apt install git`
 [참조 사이트](https://coding-factory.tistory.com/502)

##  1. Github에서 블로그 용으로 쓸 Repository 생성
Github에서 <username>.github.io 이름의 Repository 생성.

## 2. Local-Remote Repository 연동
1. Remote Repository의 주소를 복사
2. `git clone <복사한 주소> <path>`로 clone  


## 3. 테마 적용하기
1. 수많은 테마 중 **minimal mistakes**을 선택!
[minimal-mistakes Github Link](https://github.com/mmistakes/minimal-mistakes)
선택한 테마의 깃허브에 접속하여 **ZIP**파일 다운

2. 압축을 풀어주고, 안에 있는 모든 폴더 및 파일을 전부 복사

3. 2번에서 clone 했던 블로그 파일에 전부 붙여넣는다.

## 4. Github 서버와 연결해주기
1.  `git add .`
2.  `git commit -m "커밋 메세지"` 
3.  `git push origin main`


###### +  깃허브 블로그 확인하기
- 로컬에서 확인하기
`bundle exec jekyll serve` 을 실행 후,  
localhost:4000 접속
- 원격에서 확인하기
`https://깃허브아이디.github.io`에 접속


## 5. Blog customize
##### 1. 파비콘 세팅 
- 원하는 사진을 https://realfavicongenerator.net/ 에 업로드 후 압축 폴더 다운
- `_assets` 폴더에 `logo.ico` 폴더 만들어 이곳에 압축 풀기
- custom.html 수정
`github.io/_includes/_head/custom.html`
- git에 반영(add, commit, push)


##### 2. 댓글 기능 추가
1. [DISQUS](https://disqus.com/) 가입 및 세팅
2. `_config.yml` 수정
```yml
comments:
  provider    : "disqus"                                
  disqus:
    shortname : "uzinnnnnnn-github-io"                    # disqus의 shortname 기재
```
##### 3. 구글 애널리틱스 추가
https://uzinnnnnnn.github.io/
블로그에 상세 설명

