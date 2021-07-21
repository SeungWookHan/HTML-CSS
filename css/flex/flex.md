## flex 특징

- display: flex, inline-flex
- 정렬하고자 하는 요소를 감싸는 부모에서 display:flex

### flex-direction
- 가로 방향 or 세로 방향 정렬
- 가로 flex-direction: row
- 세로 flex-direction: column
- 위 설정 값에 따라 Axis 축이 달라짐

#### row
- Main axis가 좌 -> 우
- Cross axis가 상 -> 하
- reverse는 이가 반대로 됨

#### column
- Main axis가 상 -> 하
- Cross axis가 좌 -> 우
- reverse는 이가 반대로 됨

### flex-wrap
- 어떻게든 한줄 안에 모든 요소를 정렬할 것인지 or 상황에 따라 여러줄에 걸쳐 정렬할 것인지
- nowrap / wrap

---
### flex-direction에 따른 정렬 방법
- main axis에 따라서 정렬하고 프면: justify-content
    - flex-start: 왼쪽 정렬
    - center: 가운데 정렬
    - flex-end: 오른쪽 정렬
    - space-between: 사이 간격을 같게 해주기
    - space-around: 전체 왼/오 사이 사이?! 간격을 같게 해주기

- cross axis에 따라서 정렬하고 프면: align-items, align-content
    - align-items(flex: row 기준)
        - flex-start: 위쪽 정렬
        - center: 수직 방향
        - flex-end: 아래쪽 정렬
        - space-between, space-around는 사용 불가!!(여러 줄이 아니기에)
        - 하나의 flex line에 흐르는 cross-axis를 기준으로 정렬
    
    - align-content(flex: row 기준)
        - flex-wrap이 wrap이 되어야 함
        - flex-start: 위쪽 정렬
        - center: 수직 방향
        - flex-end: 아래쪽 정렬
        - space-between, space-around 사용 가능!(여러 줄로 보기에)
        - 전체 큰 흐름 cross-axis를 기준으로 정렬
    ##### 꿀팁!! 선 aligin-items 후 안되면 align-content

### order
- 각 요소의 순서를 줄 수 있음!
- flex 짱짱!!!!