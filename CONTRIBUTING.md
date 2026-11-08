# 기여 안내

Dev-Forge-Group 저장소 공통 규칙이다. 저장소에 자체 `CONTRIBUTING.md`가 있으면 그쪽을 따른다.

## 커밋·PR 작성자 표기

GitHub contributors에 AI 도구 계정이 올라가지 않도록 커밋 메타데이터에 AI 도구를 남기지 않는다.

- 커밋 메시지와 PR 본문에 AI 도구를 공동 작성자로 넣지 않는다. `Co-authored-by: Claude …`, `Co-authored-by: Codex …`처럼 `noreply@anthropic.com`·`openai.com` 주소를 쓰는 트레일러가 대상이다.
- AI 도구의 세션 링크도 넣지 않는다. `Claude-Session:` 트레일러와 PR 본문의 claude.ai 세션 URL, "Generated with …" 문구가 대상이다.
- 커밋의 author와 committer는 작업을 맡긴 사람의 Git 계정으로 한다.
- 각 저장소의 commit-attribution 검사(이 저장소의 재사용 워크플로)가 PR과 기본 브랜치 push에서 이를 확인한다. 걸리면 해당 커밋의 트레일러나 작성자를 고친 뒤 다시 push한다.

## PR

- 한 PR은 한 목적만 담는다. 형식 정리, 의존성 갱신, 기능 변경은 나눈다.
- 본문에는 무엇을 왜 바꿨는지와 확인한 방법(실행한 검사와 결과)을 적는다.
- CI가 통과한 뒤 병합한다. 실패한 검사를 끄거나 건너뛰어 통과시키지 않는다.
