<div align="center">

# 🥔 한부각감자부각

### **Now Your Thon**
### 문서만 남은 해커톤 서비스를 다시 완성하는 프론트엔드 팀

<br/>

<p>
  <img src="https://img.shields.io/badge/Daker-긴급%20인수인계%20해커톤-4F46E5?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Team-한부각감자부각-F59E0B?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Frontend-React%20%7C%20Vite-0EA5E9?style=for-the-badge" />
  <img src="https://img.shields.io/badge/State-localStorage-111827?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Deploy-Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white" />
</p>

<br/>

> **문서만 남은 서비스를, 실제로 탐색하고 팀을 구하고 제출하고 결과까지 확인할 수 있는 흐름으로 복원합니다.**

</div>

---

## ✨ 프로젝트 소개

**Now Your Thon**은  
문서만 남은 해커톤 서비스를 우리 손으로 다시 완성하겠다는 의미와,  
사용자가 자신의 해커톤 흐름을 끊기지 않고 이어갈 수 있게 만들겠다는 의미를 담은 서비스입니다.

제공된 **JSON 예시자료**, **UI 흐름도**, **메모**를 함께 분석해  
단순 소개 페이지가 아니라 아래 흐름이 실제로 이어지는 구조를 목표로 했습니다.

- 해커톤 목록 탐색
- 해커톤 상세 확인
- 팀 모집 및 팀 빌딩
- 제출 저장 및 최종 제출
- 리더보드 확인
- 전체 랭킹 확인

---

## 👋 팀 소개

**한부각감자부각**은 전원 백엔드 팀원으로 구성된 팀입니다.  
이번 해커톤에서는 사용자에게 실제로 보이는 화면과 사용 흐름까지 직접 고민하며  
**프론트엔드 영역으로 시야를 확장**하는 것을 목표로 합니다.

---

## 🎯 개발 목표

<table>
  <tr>
    <td width="50%" valign="top">

### 1. 문서 기반 서비스 복원
- 해커톤별로 분리되지 않은 공개 데이터를 `slug` 기준으로 재정리
- 목록, 상세, 팀, 제출, 리더보드를 일관된 구조로 복원
- 흩어진 데이터를 실제 사용 가능한 흐름으로 재구성

### 2. 상세 페이지 중심 허브 설계
- 개요, 안내, 평가, 일정, 팀, 제출, 리더보드가
  하나의 행동 흐름으로 이어지도록 설계
- 정보 확인만이 아니라 다음 행동까지 자연스럽게 연결

    </td>
    <td width="50%" valign="top">

### 3. 심사 친화적 구현
- 외부 키 없이 바로 확인 가능한 구조
- JSON seed + localStorage 기반 구현
- 별도 설치 없이 배포 URL만으로 전체 흐름 확인 가능

### 4. 서비스 완성도 강화
- 공통 상단 이동 구조 제공
- 로딩, 데이터 없음, 오류 상태 처리
- 실제 이용 중 막히기 쉬운 지점을 줄이는 UX 반영

   </td>
  </tr>
</table>

---

## 👥 타겟 사용자

<table>
  <tr>
    <td width="33%" align="center" valign="top">
      <h3>🏃 참가자</h3>
      어떤 해커톤에 참여할지 탐색하고<br/>
      팀까지 구해야 하는 사용자
    </td>
    <td width="33%" align="center" valign="top">
      <h3>🤝 팀장 / 팀원</h3>
      특정 해커톤과 연결해<br/>
      팀을 모집하고 제출을 준비하는 사용자
    </td>
    <td width="33%" align="center" valign="top">
      <h3>🧪 심사자 / 운영자</h3>
      배포된 URL에서 서비스 구조와 동작을<br/>
      빠르게 검토해야 하는 사용자
    </td>
  </tr>
</table>

---

## 💡 사용자에게 제공하는 가치

- 사용자는 흩어진 정보를 한곳에서 이해하고  
  **해커톤 탐색부터 팀 찾기, 제출 준비, 결과 확인까지** 끊기지 않는 흐름으로 서비스를 이용할 수 있습니다.

- 단계형 진행 안내, 제출 준비도 확인, 해커톤별 팀 연결, 점수 상세 구조가 보이는 리더보드를 통해  
  **실제 사용 중 혼동되기 쉬운 지점**을 줄일 수 있습니다.

- 단순히 화면만 만드는 것이 아니라,  
  **사용자가 서비스를 어떻게 읽고 어떻게 행동으로 이어지는지까지 책임지는 결과물**을 목표로 합니다.

---

## 🧭 페이지 구성

<table>
  <tr>
    <td width="50%" valign="top">

### `/`
**메인 페이지**
- 서비스 목적을 가장 먼저 이해하는 진입 화면
- 해커톤 보러가기, 팀 찾기, 랭킹 보기 진입점 제공
- 진행 중이거나 마감 임박 해커톤 요약 정보 노출

### `/hackathons`
**해커톤 목록**
- 제목, 상태, 태그, 시작일, 종료일 표시
- 상태/태그 필터 지원
- 마감 임박순, 최신순, 종료일순 정렬 제공

### `/hackathons/:slug`
**해커톤 상세**
- 서비스의 중심 허브 페이지
- 개요, 팀, 평가, 상금, 안내, 일정, 제출, 리더보드 제공
- 정보 확인부터 제출과 결과 확인까지 한 흐름으로 연결

    </td>
    <td width="50%" valign="top">

### `/camp`
**팀원 모집**
- 전체 팀 모집 글 탐색 및 새 팀 생성
- 특정 해커톤 기준 진입 시 해당 해커톤 팀만 필터링
- 팀명, 소개, 모집 포지션, 연락 링크, 모집 상태 표시

### `/rankings`
**랭킹 페이지**
- 개별 해커톤 리더보드와 별개로 전체 결과를 종합해 확인
- 최근 7일, 최근 30일, 전체 기준 비교 가능
- 플랫폼 전체 흐름을 한눈에 볼 수 있는 확장 페이지

### 공통 UI
- 상단 네비게이션 제공
- 로딩 / 데이터 없음 / 오류 상태 공통 처리
- 어느 페이지에서도 길을 잃지 않도록 설계

   </td>
  </tr>
</table>

---

## 🏗 시스템 구성

```text
JSON Seed Data
   ↓
Slug 기준 데이터 정리
   ↓
React Router 기반 페이지 연결
   ↓
React 컴포넌트 UI 구성
   ↓
localStorage 상태 유지
   ↓
Vercel 배포
````

---

## 🛠 기술 스택

<div align="center">

<img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
<img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white" />
<img src="https://img.shields.io/badge/React_Router-CA4245?style=for-the-badge&logo=react-router&logoColor=white" />
<img src="https://img.shields.io/badge/localStorage-334155?style=for-the-badge" />
<img src="https://img.shields.io/badge/Dummy_Data-F59E0B?style=for-the-badge" />
<img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white" />

</div>

---

## 🔧 핵심 기능

### A. 해커톤 탐색 및 워크스페이스

* 동적 필터링 시스템
* `slug` 기준 데이터 통합 상세 페이지
* 탭 기반 섹션 전환
* 저장 / 제출을 분리한 제출 폼 처리

### B. 팀 빌딩 및 캠프 시스템

* localStorage 기반 팀 생성 / 수정 / 모집 상태 변경
* 해커톤 연동 팀 필터링
* 팀 지원 / 초대 / 수락 / 거절 UI 흐름 구현

### C. 리더보드 및 랭킹 시스템

* 제출 결과 기준 자동 정렬
* 참가자 점수 + 심사위원 점수 기반 최종 점수 계산
* 기간별 랭킹 시스템
* 상위 랭커 강조 UI

### D. UX 및 예외 처리

* 로딩 / 데이터 없음 / 오류 상태 안내
* 필수 입력 검증 및 오류 방지
* 공통 네비게이션 구조 제공

---

## 🔄 주요 사용 흐름

### 사용자 흐름

```text
메인 페이지 진입
   ↓
해커톤 목록 탐색
   ↓
특정 해커톤 상세 확인
   ↓
팀 탐색 또는 팀 생성
   ↓
제출 저장 / 최종 제출
   ↓
리더보드 확인
   ↓
전체 랭킹 확인
```

### 심사자 확인 흐름

```text
배포 URL 접속
   ↓
메인 페이지에서 서비스 구조 확인
   ↓
해커톤 목록 → 상세 페이지 진입
   ↓
개요 / 일정 / 팀 / 제출 / 리더보드 검토
   ↓
팀 모집 페이지 / 랭킹 페이지 확인
   ↓
전체 서비스 흐름과 완성도 확인
```

---

## 🚨 예외 상황 및 개선 포인트

<table>
  <tr>
    <td width="50%" valign="top">

### 권한 및 인증

* 비로그인 접근 처리
* 권한 없음 안내
* 역할별 기능 제한
* 시도 시점에서 명확한 설명 제공

### 팀 빌딩 로직

* 중복 팀 참여 방지
* 정원 초과 처리
* 만료된 초대 처리
* 팀 상태 즉시 동기화

### 제출 및 시간 제약

* 마감 시간 검증
* 마감 전 / 임박 / 완료 상태 구분
* 파일 형식 및 용량 제한 검증
* 저장과 최종 제출 분리

    </td>
    <td width="50%" valign="top">

### 데이터 및 랭킹

* 집계 중 상태 안내
* 동점자 정렬 기준 유지
* 제출 완료 / 미제출 / 집계 중 상태 구분
* 새로고침 이후에도 상태 유지

### 공통 완성도 개선

* 스켈레톤 UI 기반 로딩 상태
* 데이터 없음 상태에서 다음 행동 안내
* 잘못된 slug / 만료된 요청 / 잘못된 경로 대응
* 모바일 사용성 보완

   </td>
  </tr>

</table>

---

## 🌐 Links

<table>
  <tr>
    <td align="center" width="50%">
      <h3>🚀 Deploy</h3>
      <a href="https://your-vercel-url.vercel.app">Vercel 배포 링크</a>
    </td>
    <td align="center" width="50%">
      <h3>📂 Repository</h3>
      <a href="https://github.com/onePotatoBugak/daker-handoff-hackathon">GitHub 저장소</a>
    </td>
  </tr>
</table>

---

## 🧑‍💻 Team Mission

<div align="center">

### 우리는 문서만 남은 서비스를 다시 사용 가능한 흐름으로 복원합니다

**한부각감자부각**은
흩어진 데이터와 불완전한 인수인계 자료를 해석해
탐색, 팀 빌딩, 제출, 결과 확인까지 이어지는
**실제 사용 가능한 해커톤 서비스 경험**을 만드는 팀입니다.

</div>
