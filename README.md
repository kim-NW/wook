# wook

## site => https://my-randing-page.netlify.app/

### 내가 구현한 기능 간단 소개

## 팝업창
![randing1](https://user-images.githubusercontent.com/117978017/234471243-e21a0bd9-6e65-474c-a103-76c78535c35f.png)

var a = document.getElementById("popup").style.display="inline";

`
if(a = true){
  document.querySelector('.popupcancle').addEventListener('click', function(){
    document.getElementById("popup").style.display="none";
  });
}
`

#### 처음 화면이 띄었을때 전체를 보여주는 팝업창을 띄우고 엑스를 눌르면 "display=none"으로 가려주고 랜딩페이지를 보여줌

## 햄버거 기능


![randing2](https://user-images.githubusercontent.com/117978017/234471543-ee723f17-eae9-4003-b728-061995df7d95.png)
![randing3](https://user-images.githubusercontent.com/117978017/234471564-503e60a9-8c29-405d-b742-aec9256aa2f5.png)

`
var ham = document.querySelector('.hamcontainer').style.display="none";
var hamcancle;

if(ham = true){
  document.querySelector('.navbar_tooglebtn').addEventListener('click', function(){
    document.querySelector('.hamcontainer').style.display="inline";
    var hamcancle = document.querySelector('.hamcontainer').style.display="inline";
  });
}
if(hamcancle = true){
  document.querySelector('.menu-out').addEventListener('click', function(){
    document.querySelector('.hamcontainer').style.display="none";
  });
}
`

#### 창이 줄어들어 햄버거 버튼이 생겨 햄버거 버튼을 클릭할 경우 ".hamcontainer"의 display를 inline으로 띄우줌고 "X"버튼을 누르면 none으로 가려주게 구현

## 캐러셀 기능

![스크린샷 2023-04-26 132850](https://user-images.githubusercontent.com/117978017/234482845-8fdebcb3-4cd6-4d17-a7a1-2af8723740ff.png)

`
document.querySelector('.btn01').addEventListener('click', function(){
  document.querySelector('.subcontainer').style.transform = 'translate(0vw)';
});
document.querySelector('.btn02').addEventListener('click', function(){
  document.querySelector('.subcontainer').style.transform = 'translate(-110vw)';
});
document.querySelector('.btn03').addEventListener('click', function(){
  document.querySelector('.subcontainer1').style.transform = 'translate(0vw)';
});
document.querySelector('.btn04').addEventListener('click', function(){
  document.querySelector('.subcontainer1').style.transform = 'translate(-110vw)';
});
document.querySelector('.btn05').addEventListener('click', function(){
  document.querySelector('.subcontainer2').style.transform = 'translate(0vw)';
});
document.querySelector('.btn06').addEventListener('click', function(){
  document.querySelector('.subcontainer2').style.transform = 'translate(-110vw)';
});
`

#### 사이트 자체 vw를 넓힌 다음 화면 크기만큼만 가리고, 화살표를 눌러 vw를 이동하는 코드를 구현
