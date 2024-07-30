# Git

## README

<details>
 <summary> README 작성법</summary>

#### 제목

```
# 제목1
## 제목2
...
###### 제목6 까지 있음
```

#### 줄바꿈

```
하이픈(-) 혹은 (*)을 3개 이상 적으면 구분선으로 인식
---
***
```

#### 인덱싱

```
1. 번호를 작성하면
2. 알아서
3. 만들어줌
* 순서가 1 -> 3 -> 2 이렇게 작성해도 1 -> 2 -> 3 순서대로 작성됨
```
1. 번호를 작성하면
2. 알아서
3. 만들어줌

#### 불릿

* 인덱싱과 비슷하지만 순서가 중요하지 않을 때
* +, -, * 모두 사용 가능
* tab을 이용하여 들여쓰기 가능

```
* tab 없음
  * tab 추가
```
* tab 없음
  * tab 추가

#### 텍스트 강조

* _혹은 *를 이용하여 문장을 감싸면 Italic체
* __ 혹은 **를 이용하여 문장을 감싸면 Bold체
* ___ 혹은 ***를 이용하여 감싸면 Bold + Italic체
* ~~를 이용하여 감싸면 취소선

```
_test_
__test__
___test___
~~test~~
```

_test_
__test__
___test___
~~test~~

#### 인용구

* ">"를 사용하면 인용이 된다.
* * 계속 사용 가능

```
> 한 번
> > 두 번
```

> 한 번
> > 두 번

#### 이미지 첨부

repo에 image를 upload한 뒤 이미지를 우클릭 하여 링크 주소 복사 버튼을 클릭한다.

"![이미지 이름](복사한 링크 주소)" 이런식으로 삽입

```
![test image](https://github.com/seungguJ/git/blob/master/image.png)
```

![test image](https://github.com/seungguJ/git/blob/master/image.png)

#### 접기/펼치기

```
<details>
<summary>접기/펼치기</summary>
내용
</details>
```

<details>
<summary>접기/펼치기</summary>
내용
</details>

---

<details>
<summary>reference</summary>
 
* https://velog.io/@gmlstjq123/Readme.md-%ED%8C%8C%EC%9D%BC-%EC%9E%91%EC%84%B1%EB%B2%95
* https://backendcode.tistory.com/173

</details>

</details>

## Git 사용법

<details>
 <summary> git 사용법</summary>

#### git 설치

```
sudo apt install git-all
```

#### Repository clone

```
git clone [url]
git clone --depth=1 [url] # 히스토리가 필요 없을 때 (commit 기록 다 제외하고 가장 최근 commit 된 기록만 clone)
```

#### Repository 연동 준비

연동하고 싶은 폴더로 가서 init

예를 들어 /workspace/test 폴더의 내용들을 repo와 연동시키고 싶다면

```
cd /workspace/test
git init
```

#### Repository 생성 & 연동

git 홈페이지에서 repository를 생성하고 url을 복사

```
git remote add origin [복사한 repository url] # origin이라는 이름으로 repository를 추가함
```

#### 연동된 Repository 확인

```
git remote -v # git과 연동된 repository와 이름을 확인할 수 있음
```

#### Repository의 branch 확인 및 변경

```
git branch # 로컬 브랜치 목록
git branch -M main # 브랜치를 main으로 변경
```

* 브랜치 잘 모르겠음

#### Repository에 올리기

```
git add [파일명] # git add . 하면 모든 파일 올리기
git commit -m "write message" # 커밋 메세지 작성
git push origin main # origin이름의 repo에 main branch에 push
# git push -u origin main 을 처음에 하면 이후부터는 'git push'만 하더라도 알아서 origin main에 push함
```

#### git 상태 확인 및 add 취소

현재 상태를 확인 or add 된 목록들 확인

```
git status
```

git add 취소

```
git reset [파일명] # git reset 하면 모두 add 취소
```

#### 다른 사람이 push해서 버전을 맞춰야하는 경우

```
git pull
```

<details>
<summary>reference</summary>
 
* https://wordbe.tistory.com/157

</details>

</details>
