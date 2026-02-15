# ⚡️ 번개장터 클론 코딩
<img width="1244" height="992" alt="Image" src="https://github.com/user-attachments/assets/fd5a59ce-eb40-4ee0-b5d6-b2e8817692bc" /> <br>

📅 2025.08 ~ 2025.08.03



번개장터 클론 코딩 | 여름 방학 멘토링 프로젝트

CSS, JavaScript 기초 학습 및 map 함수 기반의 동적 라우팅 구현을 목표로 진행했습니다.

반응형 웹 디자인이 개발 속도와 유지보수에 필수적임을 깨달은 프로젝트입니다.

---

# ⚙️기술적 구현

### **(1) 데이터 관리** (data.js)

- 배열로 상품 데이터 저장: `datas` 배열에 선배님이 주신 10개의 상품 객체를 저장하여 불러옴
- 각 상품 객체는 `id`, `img`, `name`, `price`, `date` 속성을 포함
- 정적 데이터를 별도 파일로 분리하여 관리

### **(2) 동적 상품 리스트 렌더링** (script.js)

- `map()` 메서드 사용: 배열의 각 상품 데이터를 순회함
- 동적 DOM 생성: `createElement()`로 상품 카드 요소 생성

```jsx
datas.map(item => {
  const div = document.createElement("div");
  div.className = "product";

  const priceWithComma = item.price.toLocaleString();

  div.innerHTML = `...`;
  container.appendChild(div);
});

```
<br>

# ‼️ 트러블 슈팅

### 1: 반응형 웹 디자인의 중요성

**문제 상황**

- 초기에 개발을 절대단위인 px로만 사용하여 데스크톱 환경 기준으로 레이아웃 구성
- 모바일이나 태블릿 등 다양한 화면 크기에서 확인했을 때 레이아웃이 깨지거나 요소들이 화면 밖으로 벗어남
- 각 화면 크기마다 `margin`과 위치를 하나하나 다 조정하려 하니 어려웠음

**해결 방법**

- 미디어 쿼리(@media) 도입으로 화면 크기별 스타일 분기 처리
- 상대 단위(`%`, `vw`, `rem` 등)와 절대 단위(`px`)를 적절하게 사용해야함


---

# 👍🏻 배운 점 및 느낀 점
- 이번 프로젝트의 주 목적은 map을 활용하여 각 영역을 클릭하면 다른 페이지로 이동할 수 있도록 만든 것이 목표였습니다.
  따라서 이번 프로젝트를 통해 map의 활용법에 대해 알게되었고  무엇보다도 개발의 속도 향상과 유지보수를 위해서는 반응형 웹 디자인은 필수가 되어야 한다는 것을 알게되었습니다.

---

## 🛠 기술 스택

<img height="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-plain.svg" /><img height="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-plain.svg" /><img height="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg" />

---

# [▶ 시연영상 확인하기](https://youtu.be/qKmHTC-8Xbw)
