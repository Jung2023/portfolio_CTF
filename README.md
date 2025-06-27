## portfolio_CTF
정보보안 포트폴리오 - CTF 대회

![CTF대회_포스터](https://github.com/user-attachments/assets/ca461fc6-922c-486b-b0a0-caf3afce9dc9)


# 🛡️ XSS-CTF & 취약점 기반 보안 실습 프로젝트

## 🔍 프로젝트 개요

- **프로젝트명:** 정보보안 CTF 대회 – CTF 머신 설계 및 공격, 방어 실습
- **수행기간:** 2025.03.13 ~ 2025.04.18
- **목표:** 실제 CTF 환경 구축 및 웹/시스템 취약점 진단·공격 실습을 통해 보안 기술 역량 강화

## 🧩 주요 활동 및 역할

### ✅ 1. CTF 환경 및 시스템 설계

- Ubuntu 기반 머신 구축
- 웹 서버 설계 (게시판, 가짜 사이트 제작 포함)
- XSS, SQL Injection, 권한 상승 등 다양한 취약점 직접 설계
- User 계정 DB 생성 및 SQL Injection 취약 설정
- `CVE-2021-3156 (sudoedit buffer overflow)` 취약점 설정
- vi/vim/nano, sudo 등 편집기 및 권한 도구 차단으로 우회 방지
- 사용자 혼란 유도용 `404 error` 웹 페이지 설계

### 🛠 2. 공격 실습 및 문제 풀이

- 타팀의 PIXEL GALLERY CTF 머신 분석 및 침투
- `nmap`, `gobuster` 등을 활용한 정보 수집
- SQL Injection 기반 계정 탈취 및 SSH 침투
- `Netcat`, `Brainfuck`, `Hex`, `stegseek` 등을 이용한 다단계 공격 시도
- 루트 권한 획득까지 완전 침투

## 🌐 프로젝트 상세 구성 (XSS-CTF)

이 저장소는 본 프로젝트에서 진행한 **XSS 취약점 중심의 웹 해킹 워게임**입니다.

- `index.php` : 기본 홈페이지
- `vuln-xss/` : XSS 취약점이 포함된 페이지들
- `flag.php` : 조건을 만족했을 때만 flag를 출력
- 다양한 XSS 스크립트 입력 시도 가능 (Reflected, Stored 등)
- 실제 공격 테스트 환경으로 활용 가능

> 🔗 GitHub 페이지 : https://github.com/Jung2023/XSS-CTF  
> 💡 Live 환경에서 로컬 PHP 서버로 직접 테스트 가능 (예: `php -S localhost:8080`)

## 🚀 핵심 보안 기술 습득

- Web Hacking: XSS, SQLi, 권한 상승 취약점 등 실전 공격 체험
- 시스템 해킹: SSH 침투, sudoedit exploit(CVE-2021-3156) 활용
- 정보 수집 및 우회 기술: gobuster, nmap, Steganography 분석
- 협업 및 문제 설계: 직접 문제 설계 및 방어 로직 구현
- 위장 및 혼란 유도 기술: 가짜 사이트, 우회 방지 로직, 404 error 페이지

## 📈 느낀점 및 성장

- 보안 취약점을 직접 설계하고 실제 침투함으로써 **보안 설계의 중요성** 체감
- 침투 테스트를 통한 **취약점 대응 역량** 향상
- 루트 권한 상승, stego 분석 등 다양한 시나리오 분석을 통해 **전반적인 시스템 보안 사고력** 제고
- **협업과 피드백을 기반으로 한 문제 해결 능력** 강화

---

## 🗂️ 프로젝트 디렉토리 예시

```bash
XSS-CTF/
├── index.php
├── vuln-xss/
│   ├── page1.php
│   ├── page2.php
├── flag.php
├── README.md
