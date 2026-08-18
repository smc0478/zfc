# ZFC

ZFC 공리계에서 출발해 집합론의 정의와 정리를 정리하고, 각 증명을 Markdown/LaTeX 문서와 Lean 4 코드로 함께 작성하기 위한 저장소입니다.

현재는 증명을 작성하기 위한 기본 구조와 LaTeX를 지원하는 GitHub Pages 배포 환경을 마련한 상태입니다.

## 작성 원칙

- 증명 문서는 `docs/` 아래에 둡니다.
- 영어 문서는 `[파일내용].md`, 한국어 문서는 `[파일내용]_kr.md` 형식으로 같은 디렉터리에 둡니다.
- 홈 문서만 예외로 한국어를 `docs/index.md`, 영어를 `docs/index_en.md`에 둡니다.
- 두 언어의 문서는 같은 정의, 정리, 증명 번호와 수식 구조를 사용합니다.
- 수식은 Markdown 안에서 LaTeX로 작성합니다.
- Lean 4 증명은 `lean/` 아래에 둡니다.
- 문서 파일명은 소문자 kebab-case, Lean 파일명은 PascalCase 사용을 기본으로 합니다.

예를 들어 하나의 정리를 작성할 때 파일은 다음처럼 대응합니다.

```text
docs/example-theorem.md
docs/example-theorem_kr.md
lean/ExampleTheorem.lean
```

## 디렉터리 구조

```text
.
├── .github/
│   └── workflows/
│       └── pages.yml          # GitHub Pages 자동 배포
├── docs/                      # Markdown/LaTeX 증명 문서
└── lean/                      # Lean 4 증명 코드
```

## 웹 문서

`docs/`를 GitHub Pages의 문서 원본으로 사용합니다. `main` 브랜치에 변경 사항을 푸시하면 GitHub Actions가 Jekyll로 사이트를 빌드하고 배포합니다.

수식은 MathJax로 표시하며 다음 문법을 사용할 수 있습니다.

```markdown
인라인 수식: $x \in A$

별도 행 수식:
$$
A \subseteq B
$$
```

최초 배포 전 GitHub 저장소의 **Settings → Pages → Build and deployment → Source**를 **GitHub Actions**로 설정해야 합니다.
