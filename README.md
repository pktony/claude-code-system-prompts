# agent-skills-zip

내 에이전트 스킬과 자주 쓰는 `.md` 를 한 곳에 모은 레포.

Claude Code 와 Codex CLI 는 같은 **Agent Skills** 규약(`SKILL.md` + frontmatter)을 쓴다.
그래서 원본은 `skills/` 한 벌만 두고, 각 에이전트의 스킬 디렉터리로 **심링크**한다.
고칠 때도 원본 하나만 고치면 되고, `git pull` 하면 양쪽에 동시에 반영된다.

설치는 [SETUP.md](SETUP.md).

## 스킬

| 스킬 | 하는 일 |
|---|---|
| [`plan-well`](skills/plan-well/SKILL.md) | 계획 문서를 쓴다 — 간결한 `PLAN.md` 1개 + 전체 흐름 다이어그램 1개 |
| [`visual-doc`](skills/visual-doc/SKILL.md) | 문서를 HTML 한 장으로 시각화한다 (20개 형식 카탈로그 기반) |

## 구조

```
skills/<name>/SKILL.md          스킬 본문. frontmatter 에 name · description 필수
skills/<name>/references/*.md   본문에서 필요할 때만 여는 참고 문서
docs/                           스킬은 아니지만 자주 쓰는 .md
```

새 스킬을 추가하거나 고칠 때의 규칙은 [AGENTS.md](AGENTS.md) 에 있다.
