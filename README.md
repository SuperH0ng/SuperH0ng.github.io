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

### - _config.yml 파일의 title을 수정하여 블로그 이름을 <b>SuperH0ng</b>으로 바꿔줌  
![image](https://user-images.githubusercontent.com/81635179/145671623-887a719f-9a99-4fa3-8854-570b4830e25e.png)  

### - header.html 파일을 수정해서 눌렀을 때 내 github, instagram, velog로 넘어가지는 링크 생성  
![image](https://user-images.githubusercontent.com/81635179/145671663-447c4470-a212-48ff-9c17-bfb6d88eff6d.png)  

### - assets > css > style.css 파일에서 각종 사진과 글씨 색, 크기, 폰트 등을 설정하여주고 각종 효과(드래그 시 색 변경, hover 속성 등)를 추가  
![image](https://user-images.githubusercontent.com/81635179/145671803-5499253c-b1a2-4a05-9012-8cf296741696.png)
