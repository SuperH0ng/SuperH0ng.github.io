# SuperH0ng.github.io

### 유레카 프로젝트 블로그 만들기

# Build 과정

## 1. Jekyll 설치 및 테스트
https://rubyinstaller.org/downloads/ 이 사이트에서 Window전용 Ruby와 DevKit(개발자 키트) 설치 프로그램을 다운로드  
` gem install jekyll bundler` 패키지 설치  
` jekyll -v`  설치 확인  
로컬 저장소로 쓸 폴더로 이동  
` jekyll new .` 지킬 기본 블로그 생성  
` jekyll serve` 지킬 실행  

위의 과정을 통해 Jekyll 환경 세팅  

## 2. 테마 포크로 받아오기
마음에 드는 지킬 테마를 찾은 후 (https://long-haul.netlify.app/)  
깃허브 주소에 들어가 내 원격저장소에 fork를 받음  
내 원격 저장소에 fork된 Repository 명을 <b>SuperH0ng.github.io</b>으로 바꿔줌  
로컬 저장소에 clone을 받으면 환경 설정 끝  

## 3. 테마 수정

* ### _config.yml 파일의 title을 수정하여 블로그 이름을 <b>SuperH0ng</b>으로 바꿔줌  
![image](https://user-images.githubusercontent.com/81635179/145671623-887a719f-9a99-4fa3-8854-570b4830e25e.png)  

* ### header.html 파일을 수정해서 눌렀을 때 내 github, instagram, velog로 넘어가지는 링크 생성  
![image](https://user-images.githubusercontent.com/81635179/145671663-447c4470-a212-48ff-9c17-bfb6d88eff6d.png)  

* ### assets > css > style.css 파일에서 글씨 색, 크기, 폰트 등을 설정하여주고 각종 효과(드래그 시 색 변경, hover 속성 등)를 추가  
![image](https://user-images.githubusercontent.com/81635179/145671803-5499253c-b1a2-4a05-9012-8cf296741696.png)

* ### assets > img 폴더에 사용하고 싶은 사진들을 넣어주고, assets > css > style.css 파일에서 불러와 사용  
![image](https://user-images.githubusercontent.com/81635179/145843795-bbfa2038-bc45-4f26-a5a4-4c9d58d2db36.png)  

* ### 각종 사용하지 않는 것들 삭제  

## 4. 포스트 작성

먼저 \_posts에 있던 기본 포스트 파일들 삭제  
마크다운 형식으로 새 파일을 만들어 나만의 post 작성  
![image](https://user-images.githubusercontent.com/81635179/145843096-f9ad947c-fcab-476c-9129-cd558d9e1757.png)  


## 5. favicon 수정  
\_includes > head.html 파일에서 favicon으로 사용할 이미지를 내가 원하는 사진 경로로 바꾸어줌  
![image](https://user-images.githubusercontent.com/81635179/145844412-71fc4293-0d0a-4244-ba8c-5038650679c8.png)  
![image](https://user-images.githubusercontent.com/81635179/145844471-48864f70-0627-4416-91f1-d3b698d32b5b.png)  
(이렇게 됨!)  

## 6. 댓글 기능 추가  
https://disqus.com << 에서 가입이 필요  

가입 중 아래 선택하는 부분에서 "I want to install Disqus on my site" 선택  
![image](https://user-images.githubusercontent.com/81635179/145849715-32706e6a-d6f9-44e1-b940-0c9a37065beb.png)  
여러가지 기입 해주기  
![image](https://user-images.githubusercontent.com/81635179/145850201-a5cb97a0-691a-4fe9-8797-b0497b5b947b.png)  
돈 없으니까 basic 골라주고, Jekyll 플랫폼 선택  
![image](https://user-images.githubusercontent.com/81635179/145850509-88b66df7-6db2-464e-93b3-46bb7fdd350e.png)  
본인 name과 웹사이트 주소에 맞게 작성  
![image](https://user-images.githubusercontent.com/81635179/145850734-f1bffcb8-3359-4820-bb8b-9dce977d2024.png)  
그 다음 쭉 넘어가고 원하는 정책 선택 여기까지 한 뒤  
Disqus 메인 페이지로 넘어간 뒤 상단 Admin > installing Disqus  
![image](https://user-images.githubusercontent.com/81635179/145851303-9efb5c13-9ac7-4887-9b1a-3ed5eda2f827.png)  
Universal Code 클릭 후 아래의 기본 코드를 수정하여 \_layouts/post.html 파일에 추가  
![image](https://user-images.githubusercontent.com/81635179/145853803-45d3b528-e43f-455d-b4ca-821758056aae.png)  
\_config.yml 파일에 아래 코드 추가  
![image](https://user-images.githubusercontent.com/81635179/145853910-4ed269a7-4475-478d-b6a2-203fdf044c30.png)  
댓글 기능을 사용하고 싶은 post 파일에 아래처럼 comments : true 코드 추가  
![image](https://user-images.githubusercontent.com/81635179/145854133-1ab028a9-c8d3-46ba-8ba6-020b608dd0cc.png)  

