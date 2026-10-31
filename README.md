# 김성진 개인 포트폴리오

컴퓨터공학을 공부하고 있는 김성진의 개인 포트폴리오 웹사이트입니다.

Hugo 정적 사이트 생성기와 Hugo Coder 테마를 활용하여 자기소개, 관심 분야, 학습 목표, 개발 프로젝트를 소개합니다.

## 사이트 및 저장소

- 사이트: https://goodabcdef.github.io/MyProfile-KSJ/
- GitHub 저장소: https://github.com/goodabcdef/MyProfile-KSJ
- 기본 브랜치: `main`

## 사이트 구성

| 페이지 | 파일 위치 | 내용 |
|---|---|---|
| 자기소개 | `site/content/about.md` | 관심 분야, 보유 역량, 학습 목표 |
| 활동 및 프로젝트 | `site/content/projects.md` | 대표 프로젝트의 개발 과정과 결과 |
| 연락처 | `site/content/contact.md` | GitHub 및 프로젝트 링크 |

## 사용 기술 및 개발 환경

- 정적 사이트 생성기: Hugo Extended 0.167.0
- 테마: Hugo Coder
- Python: 3.12
- Node.js: 24
- Go: 1.27.1
- Dart Sass: 1.105.0
- 버전 관리: Git / GitHub
- 배포: GitHub Actions / GitHub Pages

위 버전은 GitHub Actions 워크플로 설정을 기준으로 작성하였습니다.

## 프로젝트 구조

주요 파일과 디렉터리는 다음과 같습니다.

- `site/`: Hugo 사이트 프로젝트
- `site/hugo.toml`: 사이트 제목, 언어, 메뉴, SNS 설정
- `site/content/`: 자기소개 및 프로젝트 콘텐츠
- `site/static/`: 이미지 등 정적 자산
- `.github/workflows/hugo-pages.yml`: 자동 빌드 및 배포
- `.github/pages_build.py`: 배포 빌드 및 의존성 준비
- `prepare_github_pages.py`: GitHub Pages 설정 준비 스크립트
- `README.md`: 프로젝트 실행 및 관리 안내

## 로컬 실행 방법

Hugo Extended와 필요한 테마 의존성을 설치한 환경에서 저장소를 내려받습니다.

```bash
git clone https://github.com/goodabcdef/MyProfile-KSJ.git
cd MyProfile-KSJ/site
hugo server
```

개발 서버가 정상적으로 실행되면 터미널에 표시되는 로컬 주소에서 사이트를 확인합니다.

배포 빌드는 저장소 루트의 GitHub Actions 워크플로와 `.github/pages_build.py`를 통해 수행됩니다.

## 콘텐츠 수정 방법

각 페이지의 내용은 다음 파일에서 수정할 수 있습니다.

- 자기소개: `site/content/about.md`
- 프로젝트: `site/content/projects.md`
- 연락처: `site/content/contact.md`

사이트 제목, 언어, 메뉴 및 SNS 링크는 `site/hugo.toml`에서 수정합니다.

Markdown 파일을 수정한 뒤 로컬에서 변경 내용을 확인합니다.

## GitHub Pages 자동 배포

저장소의 `main` 브랜치에 변경 사항을 push하면 GitHub Actions 배포 워크플로가 자동 실행됩니다.

```bash
git add .
git commit -m "사이트 콘텐츠 및 설정 수정"
git push origin main
```

배포 확인 순서는 다음과 같습니다.

1. GitHub 저장소의 Actions 탭을 엽니다.
2. `Deploy Hugo to GitHub Pages` 실행 내역을 확인합니다.
3. 빌드와 배포 작업이 모두 성공했는지 확인합니다.
4. 공개 사이트를 열어 실제 변경 사항이 반영되었는지 검사합니다.

Actions: https://github.com/goodabcdef/MyProfile-KSJ/actions

공개 사이트: https://goodabcdef.github.io/MyProfile-KSJ/

## 사용 테마 및 출처

이 프로젝트는 Hugo Coder 테마를 기반으로 제작하였습니다.

- 테마: Hugo Coder
- 원본 저장소: https://github.com/luizdepra/hugo-coder
- 테마 저작자: Luiz de Prá 및 기여자
- 테마 라이선스: MIT License
- 라이선스 파일: https://github.com/luizdepra/hugo-coder/blob/main/LICENSE.md

테마의 기존 저작권 및 라이선스 고지를 유지합니다.

자기소개와 프로젝트 설명은 본인의 활동을 바탕으로 작성하였으며, 사이트 구성 및 문장 정리 과정에서 AI 도구의 도움을 활용하였습니다.

## 프로젝트 관리

사이트의 콘텐츠와 설정 변경 사항은 Git 커밋으로 관리합니다.

변경 사항을 적용한 뒤 GitHub Actions 실행 상태와 실제 공개 사이트를 확인하여 정상적으로 반영되었는지 검증합니다.