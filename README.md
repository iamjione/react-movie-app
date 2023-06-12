# Github pages 배포하는 법

<b>step1</b>&nbsp;&nbsp; `npm i gh-pages` 

<b>step2</b>&nbsp;&nbsp; `npm run build`   

<b>step3</b>&nbsp;&nbsp; package.json 파일에 아래 내용 추가
```
"homepage": "https://github사용자 이름.github.io/repository명" 
```
    
<b>step4</b>&nbsp;&nbsp; package.json 파일의 script에 아래 내용 추가
```
"deploy": "gh-pages -d build",
"predeploy" : "npm run build"
```  
#
변경사항 생기면 위의 과정 반복할 필요 없이 `run npm deploy` 실행하면 됨
