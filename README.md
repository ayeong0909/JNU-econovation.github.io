# 에코노베이션 블로그

IT 개발동아리 에코노베이션의 블로그입니다.

에코노베이션의 행사, 소식 등을 포스팅합니다.

## 글 작성 방법

1. 이 저장소를 fork 합니다.
2. `_posts` 폴더에 `YYYY-mm-dd-title.md`를 추가합니다.
3. 해당 파일의 상단에 아래의 내용을 추가합니다.

```
---
layout: post
title: **title 작성**
subtitle: **subtitle 작성**
author: **작성자 작성**
categories: **카테고리 작성, 띄어쓰기가 있는 경우 언더바(_)로 작성**
banner: **홈화면에 비디오 혹은 이미지를 추가하려면 작성**
  image: https://bit.ly/3xTmdUP
tags: **태그 작성, 띄어쓰기 단위로 분리됨**
sidebar: []
---
```

4. 이후 마크다운을 적용하며 포스트를 작성합니다.
5. 작성이 완료됐다면 pull request를 올려주세요. 관리자가 검토 후 merge 해드립니다.

### 주의사항

1. 이미지를 넣기 위해선 꼭 `<img src="이미지주소" alt="이미지제목" width="이미지크기(선택사항)" />`을 지켜주세요. 띄어쓰기도 꼭 지켜주시고 각 값들마다 큰따옴표도 꼭 넣어주세요.

2. 엔터를 이용한 줄바꿈도 좋지만, 문단마다의 줄바꿈을 위해 `<br/>` 태그를 추가해보세요! 글 가독성이 올라갑니다.

3. 코드 스니펫을 넣고 싶을 땐, `<pre><code class="언어">코드내용</code></pre>` 로 작성해주세요.

- 코드내용에 html 태그 등이 있으면 이스케이프 처리 후 넣어야 합니다. 그렇지 않으면 html 태그가 실제로 적용됩니다. (문자열로 처리가 되지 않습니다.)
  - ex) `<div></div>`는 `&lt;div>&lt;/div>;`와 같이 작성해야 합니다.

4. 표를 추가 하고 싶다면, `| 내용 | 내용 |` 이런식으로 하시면 됩니다. 예를들어 사진들을 표 안에 넣고 싶다면 `| <img ...> | <img ... > |` 이렇게 하시면 되고, `|` 앞뒤로 공백을 꼭 넣어주세요!

## 로컬에서 실행하기

> main으로 merge 되기 전에 글을 확인하고 싶다면, 로컬에서 실행해보세요.

- 루비 설치
- jekyll 설치
  ```
  gem install jekyll bundler
  ```
- 저장소 clone
  ```
  git clone https://github.com/JNU-econovation/JNU-econovation.github.io.git
  ```
- 실행
  ```
  jekyll serve
  ```
  또는
  ```
  bundle exec jekyll serve
  ```

## 관련 문의

문의사항이 있다면 에코노베이션 홍보부에게 문의주세요!

블로그 설정 코드 변경이 필요하다면 `jekyll` `liquid 템플릿` 등을 서칭하시면 됩니다.
