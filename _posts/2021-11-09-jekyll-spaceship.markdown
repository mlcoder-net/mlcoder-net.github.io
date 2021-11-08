---
layout: post
title:  "jekyll spaceship타고 설정블랙홀로"
date:   2021-11-08 21:06:48 +0900
categories: jekyll
---

가져와서 그냥 쓰면 된다고 하지만, 나한테 필요한 기능이 모두 있는 건 아니네요.
원하는 대로 움직이게 하려면, 세심한 배려가 필요하네요. 어렸을 땐 커스터마이징이 재미있었지만
이젠 일처럼 느껴지니..

수학이나 공학쪽 공책정리를 하다보면 그림이랑 다이어그램이랑 수식이 필요한데, jekyll 기본 기능으론
해결할 수 없고 플러그인을 설치해줘야 합니다.

[Jekyll Spaceship][jekyll-spaceship] 플러그인으로 원하는 기능이 잘 돌아가면 좋겠네요. 

### Jekyll 테스트

렌더링이 잘 되는 지 확인하고자 [jekyll-spaceship][jekyll-spaceship]에 있는 샘플코드를 따왔습니다.
로컬에선 잘 보이는 데, github 페이지에서 잘 보일지.. 

* Table 테스트

  |              Stage | Direct Products | ATP Yields |
  |-------------------:|----------------:|-----------:|
  |         Glycolysis |           2 ATP |            |
  |                 ^^ |          2 NADH |   3--5 ATP |
  | Pyruvaye oxidation |          2 NADH |      5 ATP |
  |  Citric acid cycle |           2 ATP |            |
  |                 ^^ |          6 NADH |     15 ATP |
  |                 ^^ |          2 FADH |      3 ATP |
  |         30--32 ATP |                 |            |

* MathJax

  $$
  \begin{equation}
  E = mc^2
  \end{equation}
  $$

  수식에 번호가 잘 매겨지는 보려고 `\begin{equation}`을 이용해 봤는데, 
  번호가 안 붙네요. MathJax문서 보면서 또 설정세계로 빠져야 하나. 

* PlantUML

  ```plantuml
  @startuml
  Bob -> Alice : hello
  @enduml
  ```

* Mermaid Diagram

  ```mermaid
  pie title Pets adopted by volunteers
    "Dogs" : 386
    "Cats" : 85
    "Rats" : 35
  ```

[jekyll-spaceship]: https://github.com/jeffreytse/jekyll-spaceship