# HTML

### `meta` tag

- `name` attribute

  - `title` value: 웹페이지에 대한 제목을 작성
  - `description` value: 웹페이지에 대한 설명을 작성.

  💡 위 두 값 모두 SEO(Search Engine Optimization)를 최적화할 때 사용한다.

### `<link rel="shortcut icon">`

- `rel` attribute의 `icon` value는 favicon을 적용시킬 때 사용한다.
- 종종 `icon` value 앞에 `shortcut`을 표시하는 경우가 있지만 이는 비표준이고 브라우저가 무시하기 때문에 더이상 사용하지 않는다!

  💡 Favicon을 적용할 때 `<link rel="icon" href="favicon img 경로">`만 사용하여 나타낼 수도 있다.

### `<link rel="preload">`

- `preload` value는 웹페이지에서 즉시 필요로 하는 리소스를 명시할 때 사용한다. 따라서 리소스를 더 빨리 사용할 수 있게 하고, 페이지의 렌더링을 막을 가능성이 낮아져 성능이 향상된다.

- `as` attribute를 사용하여 리소스의 유형를 알려줘야 한다. 올바른 유형이 설정되어 있지 않으면 해당 리소스는 사용되지 않는다.

### `data-*` attribute

- HTML 요소에 추가 정보를 저장할 수 있게 해준다.

  - 화면에 데이터가 보이지 않아 사용자에게 보여주지 않으면서 attribute에 데이터를 심어두고 필요할 때 마다 사용할 수 있다.

- 크롤러는 data 속성의 데이터를 읽지 못하기 때문에 주의해야 한다.

  💡 이 프로젝트에서는 JavaScript에서 해당 HTML 요소를 가져올 때 사용하였다.

### `<img loading="lazy">`

- `img` tag의 `loading` attribute는 브라우저가 이미지를 불어올 때 사용할 방식을 지정한다.

  - `eager` value: (기본값) 이미지를 즉시 불러온다.
  - `lazy` value: 특정 조건을 만족할 때 이미지를 불러온다. 일반적으로 특정 뷰포트 안에 들어올 때 불러온다. 이렇게 함으로써 불필요하게 네트워크와 저장소 대역폭을 방비하지 않을 수 있고, 또한 초기 로드 성능 향상에 도움이 된다.

<hr>

# CSS

### scroll-behavior

- 스크롤이 가능한 링크를 클릭할 때 부드럽게 움직일지 말지에 대한 여부를 지정한다.

- Values

  - `auto` (기본값): 즉시 스크롤 된다.
  - `smooth`: 부드럽게 스크롤 된다.

- `root` element에 지정하면 뷰포트에 적용된다. 하지만 `body` element에 지정하면 뷰포트에 적용되지 않는다.

### max-width

- Element의 최대 너비를 설정한다.
- 내용이 최대 너비보다 클 경우, 요소의 높이를 자동적으로 바꾼다.
- 내용이 최대 너비보다 작으면, `max-width`는 적용되지 않는다.
- `width` 속성 값이 `max-width`보다 커지는 것을 방지할 수 있다.

### transition

- CSS property 값이 변화할 때, 그 값의 변화가 일정 시간에 걸쳐 일어나도록 한다.
  [참고](https://poiemaweb.com/css3-transition)

### transform

- CSS의 스타일 변경을 부드럽게 표현하기 위해 속도를 조절한다.
  [참고](https://poiemaweb.com/css3-transform)

### box-shadow

- [참고](https://poiemaweb.com/css3-shadow)

### object-fit

- `img` 또는 `video` 요소 같은 대체 요소의 컨텐츠 크기를 어떤 방식으로 조절해 요소에 맞출 것인지 지정한다.
  [참고](https://developer.mozilla.org/ko/docs/Web/CSS/object-fit)

### margin-block

- Block에 대한 방향에 따라 여백의 크기가 달라진다.

- `margin-block-start`와 `margin-block-end`의 약식 속성이다.

- `writing-mode` 속성은 block의 뱡향을 정의한다. 따라서 `margin-block` 결과의 영향을 준다.

### padding-inline

- 테두리에서 인라인 방향의 컨텐츠까지의 공간을 의미한다. 인라인 방향에 대해 영향을 받는다.

### aspect-ratio

- 요소의 크기를 비율로 설정한다.
  [참고](https://mong-blog.tistory.com/entry/css-Aspect-Ratio-요소를-비율대로-조정하기)

### place-content

- `flex` 또는 `grid` 속성을 사용할 때, `align-content`와 `justify-content`의 약식 속성이다.

### animation

- [참고](https://poiemaweb.com/css3-animation)

### position: relative vs. absolute

- [참고](https://creamilk88.tistory.com/197)

### filter

- 그래픽 효과를 요소에 적용한다. 일반적으로 이미지, 배경, 테두리 렌더링을 조정하는데 사용된다.
  [참고](https://developer.mozilla.org/ko/docs/Web/CSS/filter)

### :is()

- 괄호 안에 selector들을 작성하여 인수로 사용하고, 해당 selector 중 선택할 수 있는 요소를 선택한다.

<hr>

# ETC

### ionicons

- 아이콘을 사용할 수 있는 오픈소스 사이트
  [ionicons](https://ionic.io/ionicons) 참고
