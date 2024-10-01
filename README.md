# 스타크래프트 노래 맞히기 유즈맵 오픈소스

Create by Myeoruchi (Heaven)
Thanks to Avlos (갈대)

## 특징
- 내가 친 정답이 다른 사람에게 보이지 않으므로, **모두가 정답**을 맞힐 수 있습니다.
- 정답자와 비정답자간에 채팅을 분리할 수 있는 **채팅 분리** 기능이 있습니다.
- 힌트 공개 여부에 따라 점수가 차등 지급됩니다.
- 스킵의 종류로 강제 스킵, 못맞힌 사람의 만장일치 스킵 투표, 다 맞힌 후 과반수 스킵 투표가 있습니다.

### Cons
- 채팅 분리 매커니즘에 의해 채팅 로그가 대부분 남지 않습니다.
- 가끔씩 채팅(정답)이 씹히는 경우가 있습니다.

## 편의 기능
전용 툴이 있으면 편할 것 같아 새로 만들었습니다.

툴의 이름은 EZDown이며 곡 다운로드, 구간 자르기, 볼륨 조절 등 다양한 기능을 수행합니다.

## 사용 방법

### 노래 다운로드
- EZDown 폴더의 엑셀 파일을 수정하여 양식에 맞게 정리하세요. (열의 이름을 바꾸어선 안됩니다.)
- EZDown 폴더의 EZDown 파일을 실행시켜 엑셀 파일의 이름과 작업할 번호 그리고 볼륨을 입력하세요.
- 작업 완료 후 자동으로 output.txt와 output_mp3 폴더에 음원 파일이 순서대로 저장됩니다.

### 노래 정보 옮기기
- output.txt 파일의 내용을 전부 복사해서 트리거 에디터 - musicInfo에 붙여넣으시면 됩니다.

### 노래 넣기
- 트리거 에디터 - 설정 - 사운드 설정에 노래 드래그 해서 넣기.
- 오프닝과 엔딩 곡은 마지막에 추가하기 (ex. 총 5곡이라면 6번째에 오프닝 곡, 7번째에 엔딩 곡)

### 힌트 시간 조절하기
- 트리거 에디터 - musicPlay에서 8번째 줄에 있는 hintTime을 수정하면 됩니다.
- 40은 첫번째 힌트, 15는 두번째 힌트 공개 시간입니다.
- 단, 음악 길이가 힌트 공개 시간보다 짧은 경우 힌트 공개에 따른 점수 차등 지급이 제대로 안될 수 있습니다.

### 제작자 이름 수정하기
- 트리거 에디터 - main에서 66번째 줄에 있는 텍스트 수정하기.
- 트리거 에디터 - opening에서 21번째 줄에 있는 텍스트 수정하기.
- input.scx에서 상단의 Scenario를 누른 후 Map Properties 및 Forces에서 수정하기.
- 오프닝과 엔딩 멘트는 각각 재량껏 수정.

### 리더보드 멘트 수정하기
- 트리거 에디터 - functions에서 65번째 줄에 있는 텍스트 수정하기.