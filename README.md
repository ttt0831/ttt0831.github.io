# ttt0831.github.io

1. 정 가운데 배치

```
display: flex;
flex-direction: column; (or row)
justify-content: center; <- 수직 가운데 정렬
align-items: center; <- 수평 가운데 정렬
text-align: center; <- 텍스트 가운데 정렬

모든 컨텐츠들이 웹 페이지의 정 가운데에 위치하게 하고싶었다.
이에 display를 flex로 만들고
수직 가운데 정렬을 해주는 justify-content: center; 와
수평 가운데 정렬을 해주는 align-items: center; 를 적용하여
정 가운데 배치를 구현할 수 있었다.



2. 메뉴에 hover하면 커지는 효과

```
.nav ul li:hover {
	transform: scale(1.4);
    transition: transform .3s;
```    
내가 누른 메뉴가 무엇인지 알게하고 싶었다.
그래서 사용자의 마우스 포인터가 요소 위에 올라가 있으면 선택되는 :hover를 사용했고
현재 선택되고 있는 요소가 무엇인지 시각적으로 알 수 있게 하기 위해 transform 속성을 이용하여 선택한 요소가 1.4배로 커지게했다.
또한 갑자기 확 커지면 자연스럽지 않으니 transition으로 애니메이션 속도를 조절했다. transition은 즉시 영향을 미치게 하지 않고, 그 속성의 변화가 일정 기간에 걸쳐 일어나도록 해준다


3. 메뉴를 누르면 해당 부분으로 이동

<li><a href="#about_me">About me</a></li>

a태그의 href속성에 해당 부분 id를 입력해주면 된다.
