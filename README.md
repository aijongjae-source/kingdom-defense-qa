# 왕국의 파수 · 비공개 QA

이 저장소는 Windows x64 QA 파일 전달용입니다. 실제 게임 파일은 **Releases의 ZIP 첨부파일**입니다. Code → Download ZIP에는 게임이 들어 있지 않습니다.

## 다운로드

[Windows QA ZIP 받기](https://github.com/aijongjae-source/kingdom-defense-qa/releases/download/qa-2026-10-25/KingdomDefense_QA_Windows_x64.zip) · [릴리스 페이지](https://github.com/aijongjae-source/kingdom-defense-qa/releases/tag/qa-2026-10-25)

로그인 없이 누구나 다운로드할 수 있습니다. ZIP 안의 ‘비공개’ 문구는 최초 전달 당시 안내이며 현재 다운로드에는 계정이 필요하지 않습니다.

## 실행

1. ZIP 전체를 압축 해제합니다.
2. `Start_QA.cmd`를 더블클릭합니다. Python/Godot 별도 설치는 필요하지 않습니다.
3. 직접 플레이 탭의 `3인 로컬 테스트 열기` 또는 자동 검사 항목을 실행합니다.
4. 여러 PC에서는 각자 `게임 창 1개 열기 (LAN)`를 선택합니다. 영주/기사/엔지니어를 다르게 고르고 호스트 LAN IPv4에 참가한 뒤, 3명 연결 후 호스트가 시작합니다. UDP 24570을 사용합니다.
5. 최초 실행 전 `VERIFY_FILES.cmd`로 무결성을 확인할 수 있습니다.

Windows 10/11 x64 / OpenGL 3.3 환경을 대상으로 합니다. 실제 다른 PC 호환은 이번 사용자 QA 대상입니다. 자동 WAN 매칭/Steam 초대는 아직 지원하지 않습니다.

## 검증 범위

다른 경로에 압축 해제하고 포함된 실행 환경으로 실제 QA 창/첫 import/첫 섬 모델97체크 및 독립3프로세스2종(core150, role_ui229) 통과를 확인했습니다. 6peer 종료0, 공통379 상태 일치, 실패/실행오류/불일치0입니다. 전체20종/정상 캠페인·실물3PC/WAN 검증을 새로 마친 것으로 보지 않습니다. 게임 전체/출시 미술은 미완성입니다.

소스 기준: `3237a66638e74754c6c86a0ab821362f83c3d573`
ZIP SHA256: `e902c77a9b07e352b425559294569a2a71de844b470b42a117d3f002140f4599`

원본 자산·Godot/Python/Tcl·Tk 고지와 한국어 실행 안내는 ZIP 안에 포함되어 있습니다.
