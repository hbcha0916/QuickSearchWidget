# QuickSearchWidget

![Untitled](QuickSearchWidget%204c24356b292e4cc6a88697c87058b862/Untitled.png)

예시사진 : 라이트모드 배경추가([https://i.pinimg.com/originals/b0/70/38/b07038309450148c02a4f08ae2a29bdf.gif](https://i.pinimg.com/originals/b0/70/38/b07038309450148c02a4f08ae2a29bdf.gif))

> QuickSearch를 위젯으로 추가해요
> 

# 기능

- QuickSearch3.0을 위젯으로 축소한 버전이에요.
- QuickSearch3.0의 핵심기능을 위젯으로도 사용할 수 있어요
    1. 빠른 붙여놓기
        
        ### 사용 방법
        
        QuickSearchWidget의 영역에 마우스를 올리고 붙여넣으면 바로 검색이 가능해요.
        
    2. 빠른 검색
        
        ### 사용 방법
        
        검색창에 검색어를 입력해요.
        

# 주의

QuickSearchWidget은 Tistory스킨 hELLO 을 기준으로 개발되었습니다.

[https://pronist.tistory.com/5](https://pronist.tistory.com/5)

# 기본 모습

![다크모드](QuickSearchWidget%204c24356b292e4cc6a88697c87058b862/Untitled%201.png)

다크모드

![라이트모드](QuickSearchWidget%204c24356b292e4cc6a88697c87058b862/Untitled%202.png)

라이트모드

원본소스에는 배경화면을 적용하지 않았습니다.

# 적용 방법

1. 티스토리 ‘배너 출력’ 플러그인을 적용시켜 주세요.

![Untitled](QuickSearchWidget%204c24356b292e4cc6a88697c87058b862/Untitled%203.png)

1. 그 다음 ‘꾸미기’ → ‘사이드바’ 에서 ‘html 배너출력’ 을 추가해 주세요.
2. 그 다음 추가해준 ‘html 배너출력’ 에서 ‘편집’버튼을 클릭해주세요.
3. ‘이름’은 지정해 주시고 ‘html 소스’에 아래 내용을 넣어 주세요.
    
    ### 라이트 / 다크모드
    
    사용자 컴퓨터가 라이트/다크모드 일 경우 자동으로 바뀌는 플러그인
    
    ```html
    <iframe src="https://astonishing-pegasus-8edb41.netlify.app/"  style="background-image: url('여기 따옴표 안에 배경화면 url을 넣어 주세요.');">
        <h3>이 브라우저는iFrame을 지원하지 않습니다.</h3>
    </iframe>
    ```
    
    ### 라이트 모드
    
    사용자 컴퓨터가 다크모드 이더라도 이 플러그인은 항상 라이트 모드입니다.
    
    ```html
    <iframe src="https://hbchaquicksearch-widget-white.netlify.app/"  style="background-image: url('여기 따옴표 안에 배경화면 url을 넣어 주세요.');">
        <h3>이 브라우저는iFrame을 지원하지 않습니다.</h3>
    </iframe>
    ```
    
    ### 다크 모드
    
    사용자 컴퓨터가 라이트모드 이더라도 이 플러그인은 항상 다크모드 입니다.
    
    ```html
    <iframe src="https://hbchaquicksearch-widget-black.netlify.app/"  style="background-image: url('여기 따옴표 안에 배경화면 url을 넣어 주세요.');">
        <h3>이 브라우저는iFrame을 지원하지 않습니다.</h3>
    </iframe>
    ```
    

# 배경화면 적용 방법

위 코드에서 `'여기 따옴표 안에 배경화면 url을 넣어 주세요.'` 부분에 배경화면 URL을 삽입합니다.

- 배경화면은 `235 x 190` 사이즈 이하를 권장합니다.
- 배경화면을 적용하지 않을 시 블로그 사이드바 스킨 성격을 가집니다.