# Webfont Test 

안녕하세요. 웹폰트 테스트 페이지 사용법을 알려드립니다 :)

Hello. I'm telling you how to use the web font test page :)


# How to Use
일단 [GitHub/webfont_test](https://github.com/tvfxq0213/webfont_test) 페이지 에서 **code 버튼 클릭 >  download ZIP** 을 눌러 가장 최신 버전의 파일을 다운로드 합니다.
Once on the [GitHub/webfont_test](https://github.com/tvfxq0213/webfont_test) page, click the **code button > download ZIP** to download the latest version of the file.

 - 압축된 파일을 다운로드 후 index.html 파일을 테스트할 브라우저로 열어주세요 (브라우저를 따로 설정하지 않는다면 컴퓨터에 설정된 기본 브라우저로 열리게 됩니다)
 - 파일을 브라우저에서 열면 아래와 같은 화면이 나타나게 됩니다. 현재 샘플페이지에 적용되어 있는 폰트는 ‘GothicA1’ 으로([Google Fonts: Gothic A1](https://fonts.google.com/specimen/Gothic+A1?subset=korean&noto.script=Kore) ) 구글에서 적용하는 한글용 폰트중 9개의 웨이트가 모두 존재하여 다양한 웨이트의 웹폰트를 보여주기 위해 선택하였습니다.

 - 폰트를 변경하고 싶다면 압축을 푼 폴더 안에 style 폴더로 들어간후 style.css 를 열여주세요. 윈도우는 “메모장” 맥은 “텍스트 편집기”를 이용해서 파일을 열면 되고, 혹시 notepad++, vscode, atom 등의 코드 편집프로그램이 있다면 편한 것으로 열어주세요.
 - 텍스트 편집기를 통해 파일을 열면 아래와 같은 화면이 뜨게 됩니다. 변경된 폰트에 따라 보라색 영역을 수정해야 웹화면에서 보여질 폰트를 수정할 수 있습니다.

 - 먼저 적용할 폰트를 압축을 푼 폴더의 fonts 폴더안에 넣어주세요
 -  font-family 명을 적용할 폰트 명으로 바꿔줍니다. 아래 body에 있는 font-family까지 변경해주세요
 - 웨이트별로 해당하는 파일 경로 부분을 해당하는 웨이트별 파일로 변경해주세요 , 파일 확장자나 대소문자도 꼭 확인해서 맞게 넣어주세요!


 src: url("../fonts/GothicA1-Light.ttf"); 2src: local(※), url("../fonts/GothicA1-Light.ttf") format("woff");

 - 위 파일을 저장한후 index.html 파일을 새로고침해주세요. 웹폰트가 적용되어 있다면 완료입니다!

 - 만약 웹폰트가 적용되어 있지 않다면 브라우저에서 마우스오른쪽버튼 > 검사 를 눌러보세요 (크롬 기준) 웹페이지의 하단이나 오른쪽의 영역에 아래같은 영역이 생기기도 하고, 새창으로 뜨기도 합니다.
 - 하단 빨간영역에 오류가 발생하고, 빨간 텍스트가 들어온다면, 폰트 파일을 제대로 불러오지 못하고 있는 것입니다. style.css에서 다시 파일 경로를 확인해주세요
 - 오류메세지가 없는데 적용되지 않는다면 “계산됨(또는 Computed)” 탭을 눌러 렌더링된 글꼴이 적용한 폰트가 맞는지 확인해주세요
 - 렌러딩된 글꼴이 네트워크 리소스 이어야 합니다. 로컬리소스로 되어있다면 이미 컴퓨터에 설치되어 있는 폰트를 불러오는것이라 제대로 적용되고 있는 것이 아닙니다.
