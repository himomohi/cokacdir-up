# COKACDIR

[English](README.md) | [한국어](README.ko.md)

AI 자연어 명령을 지원하는 멀티 패널 터미널 파일 매니저입니다.

**터미널이 어려운 바이브 코더를 위한 터미널 파일 매니저** - 터미널이 익숙하지 않아도 쉽게 탐색할 수 있습니다.

## 주요 기능

- **매우 빠른 성능**: Rust로 작성되어 높은 성능을 제공합니다. 약 10ms 시작 속도, 약 5MB 메모리 사용량, 약 4MB 정적 바이너리(런타임 의존성 없음).
- **AI 명령 지원**: Claude & Codex 기반 자연어 파일 작업을 지원합니다. `.` 키를 누르고 원하는 작업을 설명하세요.
- **멀티 패널 탐색**: 동적 멀티 패널 인터페이스로 파일을 효율적으로 관리할 수 있습니다.
- **키보드 중심 조작**: 파워 유저를 위한 전체 키보드 네비게이션.
- **내장 편집기**: 20개 이상 언어의 문법 하이라이팅을 지원하는 파일 편집기.
- **이미지 뷰어**: 터미널에서 이미지 확대/이동(Zoom/Pan) 지원.
- **프로세스 매니저**: 시스템 프로세스 모니터링 및 관리.
- **파일 검색**: 이름 패턴 기반 재귀 검색.
- **Diff 비교**: 폴더/파일을 나란히 비교.
- **Git 통합**: git status, commit, log, branch 관리 및 커밋 간 diff 지원.
- **원격 SSH/SFTP**: 저장된 프로필로 원격 서버 탐색.
- **파일 암호화**: AES-256 암호화 및 청크 분할 설정 지원.
- **테마 커스터마이징**: 라이트/다크 테마와 상세 색상 설정 지원.

## 설치

### 빠른 설치 (권장)

```bash
/bin/bash -c "$(curl -fsSL https://cokacdir.cokac.com/install.sh)"
```

설치 후 실행:

```bash
cokacdir [PATH...]
```

경로를 여러 개 넘겨 멀티 패널로 열 수 있습니다:

```bash
cokacdir ~/projects ~/downloads ~/documents
```

### 소스에서 빌드

```bash
# 저장소 복제
git clone https://github.com/kstost/cokacdir.git
cd cokacdir

# 릴리스 빌드
cargo build --release

# 실행
./target/release/cokacdir
```

자세한 빌드 방법은 [build_manual.md](build_manual.md)를 참고하세요.

## AI 명령 활성화 (선택)

자연어 파일 작업을 사용하려면 Claude Code 또는 Codex CLI를 설치하세요.

```bash
# Claude Code
npm install -g @anthropic-ai/claude-code

# Codex CLI
npm install -g @openai/codex
```

자세한 정보: [Claude Code](https://docs.anthropic.com/en/docs/claude-code) | [Codex CLI](https://github.com/openai/codex)

## 문서

상세 사용법, 단축키, 튜토리얼:

**[https://cokacdir.cokac.com/#/tutorial](https://cokacdir.cokac.com/#/tutorial)**

## 지원 플랫폼

- macOS (Apple Silicon & Intel)
- Linux (x86_64 & ARM64)
- Windows (x86_64 & ARM64)

## 라이선스

MIT License

## 작성자

cokac <monogatree@gmail.com>

홈페이지: https://cokacdir.cokac.com

## 면책 조항

이 소프트웨어는 상품성, 특정 목적 적합성, 비침해성에 대한 보증을 포함하되 이에 한정되지 않는 어떠한 명시적/묵시적 보증 없이 "있는 그대로(AS IS)" 제공됩니다.

어떠한 경우에도 작성자, 저작권자 또는 기여자는 계약, 불법행위 또는 기타 법적 근거와 무관하게 이 소프트웨어의 사용 또는 기타 취급으로 인해 발생하는 모든 청구, 손해 또는 기타 책임에 대해 책임지지 않습니다.

여기에는 아래 항목이 포함되나 이에 한정되지 않습니다.

- 데이터 손실 또는 손상
- 시스템 손상 또는 오작동
- 보안 침해 또는 취약점
- 금전적 손실
- 직접, 간접, 부수적, 특별, 징벌적 또는 결과적 손해

사용자는 본 소프트웨어 사용으로 인해 발생하는 모든 결과에 대해 전적인 책임을 집니다. 해당 사용이 의도되었는지, 승인되었는지, 예상되었는지와 관계없이 동일합니다.

**사용에 따른 모든 책임은 사용자에게 있습니다.**
