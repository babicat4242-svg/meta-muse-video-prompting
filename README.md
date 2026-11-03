# Meta Muse Video Prompting Skill

메타 Muse Video용 한국어 영상 프롬프트 스킬입니다. Claude와 Codex에서 사용합니다.

## 설치·호출

- Claude Code: `meta-muse-video-prompting` 폴더 전체를 `~/.claude/skills/`에 복사하고 `/meta-muse-video-prompting`으로 호출합니다.
- Codex: 같은 폴더를 `~/.codex/skills/`에 복사하고 `$meta-muse-video-prompting`으로 호출합니다.
- Claude 웹·데스크톱: [사용자 스킬 업로드 ZIP](dist/meta-muse-video-prompting-claude.zip)을 다운로드해 사용자 스킬로 등록·활성화합니다. 업로드 기능의 제공 여부는 계정·조직 설정에 따릅니다.

`references/`도 함께 설치합니다. ZIP은 스킬 폴더를 루트로 가지며 Codex 전용 UI 메타데이터는 제외했습니다.

## 요청 예

“Meta Muse Video 스킬로 첨부 이미지 기반 5초 장면 프롬프트를 작성해줘. 인물이 팔을 들어 유니콘을 쓰다듬고, 배경음악 없이 현장음만 들리게 해줘.”

실제 생성 길이와 이미지 입력 지원은 현재 서비스에서 확인합니다. 프롬프트 작성에는 영상 생성 연결이 필요하지 않습니다.

## 포함 내용

- 씨댄스 2.5에서 각색한 인물 행동·감정·접촉·카메라·조명·VFX·연속성
- 영화·판타지·광고·뮤직비디오 장면 구성
- NO BGM·완전 무음·원본 오디오·무반주 보컬 구분
- 시간과 조건 변경 시 전체 프롬프트 재작성
- 요청 시 제작 브리프 JSON 출력
- Muse Image·Spark·개인 비서와 Muse Video 기능 구분

Meta 공식 배포본이 아닌 개인 작성 스킬입니다. 전체 씨댄스 사례집을 복제하지 않았으며, 공개 문서에서 확인되지 않은 Muse Video API·길이·한도를 만들어 넣지 않았습니다.

검증: 구조·상대 링크·ZIP 구성 확인. 실제 Claude 업로드나 Muse 영상 생성 성공을 검증한 것은 아닙니다.

## 공식 참고

- [Meta Muse Image·Video 소개](https://ai.meta.com/blog/introducing-muse-image-muse-video-msl/)
- [Meta Model API](https://dev.meta.ai/docs/overview)
- [Claude Code 스킬](https://code.claude.com/docs/en/skills)
- [Claude 사용자 스킬](https://support.claude.com/en/articles/12512198-how-to-create-custom-skills)

문서 확인일: 2026-11-02.
