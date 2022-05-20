# __Git__

## 디렉토리에서 깃을 쓰려면   
```git
git init
```
<br/>

## 파일 스테이징 하는 법   
```git
git add "파일 이름"
```
&ensp; &ensp; 
"파일 이름"에 *을 쓰면 모든 파일.

<br/>

## 커밋하는 법   
```git
git commit -m "커밋 메시지"
```
<br/>

## 브랜치 만들고 이동하는 법   
```git
git checkout -b "브랜치 이름"
```
<br/>

## Github 경로 추가하는 법   
```git
git remote add "경로 이름" "URL"
```
&ensp; &ensp; local repo A에서 P라는 경로를 추가했어도 local repo B에서 쓸 수 없다.    
&ensp; &ensp; B에서 쓰려면 B에서 추가해줘야 한다.

## remote repository에서 가져오는 법
### &ensp; &ensp; git clone을 쓰는 방법
```git
git clone "경로 이름"

git clone -b "브랜치 이름" --single-branch "URL"
```
&ensp; &ensp; git clone을 쓰면 통째로 가져온다.   
&ensp; &ensp; 현재 로컬에서의 내 브랜치가 어디든 상관없이.   
<br/>

### &ensp; &ensp; git pull을 쓰는 방법
```git
git pull "경로 이름" "브랜치 이름"
```
&ensp; &ensp; git pull을 쓰면 원격 저장소 브랜치의 파일만 가져오고   
&ensp; &ensp; 현재 브랜치를 유지한다.   

&ensp; &ensp; *그래서 pull 한 브랜치에 push 하고 싶으면   
&ensp; &ensp; pull 하기 전에 현재 위치한 브랜치 이름을   
&ensp; &ensp; pull 하는 브랜치랑 같게 만들어 주어야 한다.*

&ensp; &ensp; *pull = fetch + merge   
&ensp; &ensp; fetch > 업데이트 정보만 가져옴   
&ensp; &ensp; merge > 그 정보에 따라서 파일을 가져와서 합침*