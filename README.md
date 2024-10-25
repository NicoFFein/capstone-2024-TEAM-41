### 1. 프로젝트 소개

#### 1.1. 배경 및 필요성

녹내장은 눈 속의 압력이 증가하여 시신경이 손상되고 부분적 또는 완전한 시력 손실로 이어질 수 있는 심각한 안과 질환입니다.
이 연구는 딥러닝 기반 특징 추출을 통해 초기 단계에서 녹내장을 감지하는 것을 목표로 합니다. 망막 또는 안저 이미지는 눈 질환을 감지하는 데 중요한 소스입니다. 녹내장의 주요 원인은 눈의 형태를 유지하는 액체의 양의 불균형으로 인해 시신경유두(ONH)에 가해지는 압력이 증가하여 손상을 초래하는 것입니다. 안저 이미지를 분석하여 녹내장을 조기에 감지할 수 있는 AI 모델을 개발하고, 이를 통해 환자의 예후를 개선하고 시력 손실의 위험을 줄이는 것을 목표로 하고 있습니다.

#### 1.2. 목표 및 주요 내용

본 연구의 주요 목표는 다음과 같습니다:

- 녹내장 조기 발견: 망막 안저 이미지를 활용하여 초기 단계에서 녹내장을 감지할 수 있는 딥러닝 기반 시스템을 개발합니다.

- 전처리 및 분할: 이미지 품질 향상 및 잡음 감소를 위한 전처리 기법을 구현하고, OC 마스크가 없는 데이터셋에서 관심 영역(ROI)을 추출하기 위한 분할 작업을 수행합니다.

- 특징 추출: 컨볼루션 신경망(CNN), 로컬 이진 패턴(LBP), 방향성 그래디언트 히스토그램(HOG), 가속화된 강인 특징(SURF)과 같은 하이브리드 특징 기술을 사용하여 시신경 유두(OD) 및 시신경 컵(OC) 영역에서 세부적인 특징을 추출합니다.

- 특징 선택 및 순위 매기기: MR-MR 방식을 사용하여 가장 대표적인 특징을 선택하고 순위를 매겨 효율적이고 정확한 특징 표현을 보장합니다.

- 분류: 서포트 벡터 머신(SVM), 랜덤 포레스트(RF), K-최근접 이웃(KNN)과 같은 다중 클래스 분류기를 사용하여 안저 이미지를 건강한 상태와 질환 상태로 분류합니다.

- 성능 평가: 제안된 시스템의 성능을 평가하기 위한 다양한 실험을 수행하여 녹내장 조기 발견에서 높은 정확도를 목표로 합니다.
  
### 2. 상세설계

### 5. 팀 소개
| Name              | Contact Information     | Roles                                                   | 
|-------------------|-------------------------|---------------------------------------------------------|
| Nemekhbayar Nomin | sharon.nemhee@gmail.com | 데이터 수집, 특징 추출 알고리즘 구현, 분류 알고리즘 구현    |
| Battulga Bazarsad | nicoffeingg@gmail.com   | 이미지 전처리, 관심 영역(ROI) 감지, 특징 선택 알고리즘 구현 |







## 1. 레파지토리 생성
- [https://classroom.github.com/a/NJK_cPkH](https://classroom.github.com/a/NJK_cPkH)
- 위 Github Classroom 링크에 접속해 본인 조의 github 레파지토리를 생성하세요.
<img src="https://github.com/user-attachments/assets/b5a7f34a-e146-4253-b57d-672737a75a50" alt="깃헙 클래스룸 레포 생성" width="600" />

- 레포지토리 생성 시 팀명은 `TEAM-{조 번호}` 형식으로 생성하세요.
- 예를 들어, 2024년도 3조의 팀명은 `TEAM-03` 입니다.
- 이 경우 `Capstone2024-TEAM-03`이란 이름으로 레파지토리가 생성됩니다.

---

## 2. 레파지토리 구성
- 레파지토리 내에 README.md 파일 생성하고 아래의 가이드라인과 작성팁을 참고하여 README.md 파일을 작성하세요. (이 레파지토리의 SAMPLE_README.md 참조)
- 레파지토리 내에 docs 디렉토리를 생성하고 docs 디렉토리 내에는 과제 수행 하면서 작성한 각종 보고서, 발표자료를 올려둡니다. (이 레파지토리의 docs 디렉토리 참조)
- 그 밖에 레파지토리의 폴더 구성은 과제 결과물에 따라 자유롭게 구성하되 가급적 코드의 목적이나 기능에 따라 디렉토리를 나누어 구성하세요.

---

## 3. 레파지토리 제출 

- **`[주의]` 레파지토리 제출**은 해당 레파지토리의 ownership을 **학과 계정**으로 넘기는 것이므로 되돌릴 수 없습니다.
- **레파지토리 제출** 전, 더 이상 수정 사항이 없는지 다시 한번 확인하세요.
- github 레파지토리에서 Settings > General > Danger zone > Transfer 클릭
  <img src="https://github.com/user-attachments/assets/cb2361d4-e07e-4b5d-9116-aa80dddd8a8b" alt="소유주 변경 경로" width="500" />
  
- [ Specify an organization or username ]에 'PNUCSE'를 입력하고 확인 메세지를 입력하세요.
  <img src="https://github.com/user-attachments/assets/7c63955d-dcfe-4ac3-bdb6-7d2620575f3a" alt="소유주 변경" width="400" />

---

## 4. README.md 가이드 라인
- README 파일 작성시에 아래의 5가지 항목의 내용은 필수적으로 포함해야 합니다.
- 아래의 5가지 항목이외에 프로젝트의 이해를 돕기 위한 내용을 추가해도 됩니다.
- SAMPLE_README.md 이 단순한 형태의 예제이니 참고하세요.

```markdown
### 1. 프로젝트 소개
#### 1.1. 배경 및 필요성
> 프로젝트를 실행하게 된 배경 및 필요성을 작성하세요.

#### 1.2. 목표 및 주요 내용
> 프로젝트의 목표 및 주요 내용을 작성하세요.

### 2. 상세설계
#### 2.1. 시스템 구성도
> 시스템 구성도(infra, front, back등의 node 간의 관계)의 사진을 삽입하세요.

#### 2.1. 사용 기술
> 스택 별(backend, frontend, designer등) 사용한 기술 및 버전을 작성하세요.
> 
> ex) React.Js - React14, Node.js - v20.0.2

### 3. 설치 및 사용 방법
> 제품을 설치하기 위헤 필요한 소프트웨어 및 설치 방법을 작성하세요.
>
> 제품을 설치하고 난 후, 실행 할 수 있는 방법을 작성하세요.

### 4. 소개 및 시연 영상
> 프로젝트에 대한 소개와 시연 영상을 넣으세요.

### 5. 팀 소개
> 팀원 소개 & 구성원 별 역할 분담 & 간단한 연락처를 작성하세요.
```

## 5. README.md 작성팁 
* 마크다운 언어를 이용해 README.md 파일을 작성할 때 참고할 수 있는 마크다운 언어 문법을 공유합니다.  
* 다양한 예제와 보다 자세한 문법은 [이 문서](https://www.markdownguide.org/basic-syntax/)를 참고하세요.

### 5.1. 헤더 Header
```
# This is a Header 1
## This is a Header 2
### This is a Header 3
#### This is a Header 4
##### This is a Header 5
###### This is a Header 6
####### This is a Header 7 은 지원되지 않습니다.
```
<br />

### 5.2. 인용문 BlockQuote
```
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.
```
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.
<br />

### 5.3. 목록 List
* **Ordered List**
```
1. first
2. second
3. third  
```
1. first
2. second
3. third
<br />

* **Unordered List**
```
* 하나
  * 둘

+ 하나
  + 둘

- 하나
  - 둘
```
* 하나
  * 둘

+ 하나
  + 둘

- 하나
  - 둘
<br />

### 5.4. 코드 CodeBlock
* 코드 블럭 이용 '``'
```
여러줄 주석 "```" 이용
"```
#include <stdio.h>
int main(void){
  printf("Hello world!");
  return 0;
}
```"

단어 주석 "`" 이용
"`Hello world`"

* 큰 따움표(") 없이 사용하세요.
``` 
<br />

### 5.5. 링크 Link
```
[Title](link)
[부산대학교 정보컴퓨터공학부](https://cse.pusan.ac.kr/cse/index..do)

<link>
<https://cse.pusan.ac.kr/cse/index..do>
``` 
[부산대학교 정보컴퓨터공학부](https://cse.pusan.ac.kr/cse/index..do)

<https://cse.pusan.ac.kr/cse/index..do>
<br />

### 5.6. 강조 Highlighting
```
*single asterisks*
_single underscores_
**double asterisks**
__double underscores__
~~cancelline~~
```
*single asterisks* <br />
_single underscores_ <br />
**double asterisks** <br />
__double underscores__ <br />
~~cancelline~~  <br />
<br />

### 5.7. 이미지 Image
```
<img src="image URL" width="600px" title="Title" alt="Alt text"></img>
![Alt text](image URL "Optional title")
```
- 웹에서 작성한다면 README.md 내용 안으로 이미지를 드래그 앤 드롭하면 이미지가 생성됩니다.
- 웹이 아닌 로컬에서 작성한다면, github issue에 이미지를 드래그 앤 드롭하여 image url 을 얻을 수 있습니다. (URL만 복사하고 issue는 제출 안 함.)
  <img src="https://github.com/user-attachments/assets/0fe3bff1-7a2b-4df3-b230-cac4ef5f6d0b" alt="이슈에 image 올림" width="600" />
  <img src="https://github.com/user-attachments/assets/251c6d42-b36b-4ad4-9cfa-fa2cc67a9a50" alt="image url 복사" width="600" />


### 5.8. 유튜브 영상 추가
```markdown
[![영상 이름](유튜브 영상 썸네일 URL)](유튜브 영상 URL)
[![부산대학교 정보컴퓨터공학부 소개](http://img.youtube.com/vi/zh_gQ_lmLqE/0.jpg)](https://www.youtube.com/watch?v=zh_gQ_lmLqE)    
```
[![부산대학교 정보컴퓨터공학부 소개](http://img.youtube.com/vi/zh_gQ_lmLqE/0.jpg)](https://www.youtube.com/watch?v=zh_gQ_lmLqE)    

- 이때 유튜브 영상 썸네일 URL은 유투브 영상 URL로부터 다음과 같이 얻을 수 있습니다.

- `Youtube URL`: https://www.youtube.com/watch?v={동영상 ID}
- `Youtube Thumbnail URL`: http://img.youtube.com/vi/{동영상 ID}/0.jpg 
- 예를 들어, https://www.youtube.com/watch?v=zh_gQ_lmLqE 라고 하면 썸네일의 주소는 http://img.youtube.com/vi/zh_gQ_lmLqE/0.jpg 이다.

