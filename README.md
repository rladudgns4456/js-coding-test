# 🧠 JavaScript Coding Test Solutions

자바스크립트 기반 코딩테스트 문제 풀이 아카이브입니다.  
각 문제는 폴더 단위로 구성되어 있으며, 문제 설명과 접근 방식은 `README.md`, 코드 해설은 `solution.js`에 포함되어 있습니다.

## 📂 폴더 구조

```bash
js-coding-test/
├─ 01_two_sum/
│   ├─ solution.js
│   └─ README.md
├─ 02_valid_parentheses/
│   ├─ solution.js
│   └─ README.md
└─ README.md ← 이 파일
```

## ✅ 풀이 목록

| 번호 | 문제 이름             | 링크 |
|------|----------------------|------|
| 01   | Two Sum              | [바로가기](./01_two_sum/README.md) |
| 02   | Valid Parentheses    | [바로가기](./02_valid_parentheses/README.md) |


---

## 📌 예시: 문제 디렉토리 README 템플릿

```markdown
# 🧮 01. Two Sum

## 📌 문제 설명
정수 배열 `nums`와 정수 `target`이 주어졌을 때,
합이 `target`이 되는 두 수의 인덱스를 반환하라.

## 💡 접근 방식
- 해시맵을 이용한 보완 탐색
- 시간 복잡도: O(n)

## ✅ 풀이 코드

```js
function twoSum(nums, target) {
  const map = {};
  for (let i = 0; i < nums.length; i++) {
    const complement = target - nums[i];
    if (map[complement] !== undefined) {
      return [map[complement], i];
    }
    map[nums[i]] = i;
  }
}
```
```

---

## 📌 사용 기술

- JavaScript (ES6+)
- Node.js (테스트용)

## 🧩 진행 방식

- [ ] 매일 1~2문제 풀이 업로드
- [ ] 각 문제 별 접근법 정리
- [ ] 고난도 문제에는 시간복잡도 및 개선 아이디어 추가

---

## 📬 Contact

- GitHub: [@rladudgns4456](https://github.com/rladudgns4456)
- Email: rladudgns4456@gmail.com
