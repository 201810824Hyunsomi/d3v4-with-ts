# d3v4-with-ts

### react 와 d3 사용하기 

    
    1. react가 d3에게 dom을 제공하고 d3는 이것을 받아 데이터를 화면에 보여주어 react hook으로 상태를 관리하고 d3로 데이터 시각화를 진행한다.사용자가 화면상에서 데이터를 조작했을 때 변경된 데이터로 화면에 다시 document를 그릴 수 있어 대화형 데이터 시각화를 구축할 수 있다.
    2.react 프로젝트 폴더에 d3패키지 설치하기 
    npm i -S d3@^4.13.0(설치)
    npm i -D typescript@^2.4.2
    npm i -D @types/d3@^4.10.0
    

### d3 동작과정 


    1. loading 보여줄 데이터를 불러온다.
    2. selecting-binding 시각적 요소 안에 데이터 수치를 입력한 코드에 맞춰 연동시킨다.
    3. transform : 그래프의 다양한 요소를 정해준다.
    4. transition : 클릭, 드래그 등 인터렉션 효과를 지정한다.
    
    
### d3 메서드 체인 

    메서드를 체인으로 연결하는 순서가 중요한데 . 과 함께 체인처럼 연결해 한줄에 여러 동작을 실행할 수 있는 기법이다.
    d3. select-현재 문서에서 특정 태그 하나를 선택하는 메서드
    d3.selectAll- 특정 태그 전체를 선택
    data - 참조 연결할 데이터를 가져옴
    enter- 데이터 개수만큼 태그가 부족할때 부족한 수만큼 플레이스 홀더를 반환함
    append 태그 추가
    exit 필요없는 태그 반환 
    remove: 선택된 태그를 제거
    
    
    
### svg(scalable vector graphics) 
    
    
    웹용 벡터 그래픽으로 html 문서에 직접 포함할 수 있다.
    코드 작업으로 이미지 편집이 가능하며, 품질 손상없이 확대 및 축소가 가능하다.
    
    
  
### d3로 dot 차트 만들기


    1. 개발환경 세팅/ 타입스크립트 컴파일 환경 세팅
    Roll-up을 이용한 bundling- 브라우저가 이해하는 형태로 변경
    서비스 시작하기 (live –server 설치)
    Ts파일 변화를 감시해서 ts 파일 변경 후 브라우저 내용 변경요청
    
    2. Reddit API를 사용해 스코어를 표현하기
    <차트 구성>- the svg, the plot area, the axes, the points

    <단계> svg 만들기
    Plot area 만들기
    Plot area에 x축 그룹 추가
    Plot area에 y축 그룹 추가
    데이터 포인트 그룹 추가

        
### 세로형 막대그래프 표현 
    
    
    1. 막대형 그래프에 수치 표현, 눈금 표현 
### 체크박스 표현

### 선 그래프 표현
