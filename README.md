# gameserver-resourcepack

개인 마인크래프트 서버(Paper 26.1.2)의 필수 리소스팩이다. 서버에 들어올 때 자동으로 받는다.

## 담은 것
- 가짜 플레이어 블록의 겉모습: 얼굴 화면이 달린 강철 상자
- 상태별 그림
  - 인벤토리 아이템: 하늘색 얼굴
  - 작동 중: 초록색 웃는 얼굴
  - 쉬는 중(서버 부하 보호로 잠시 멈춤): 호박색 졸린 얼굴
  - 꺼둠(주인이 끔): 회색 전원 기호
- 무선 레드스톤 송신기·수신기의 겉모습: 같은 강철 상자에 구리 리벳
  - 송신기: 옆면에 가운데 점에서 바깥으로 퍼지는 전파 호 두 겹, 윗면에 구리 안테나 꼭지
  - 수신기: 옆면·윗면에 과녁 무늬 동심원
  - 꺼짐(신호 0)은 어두운 빨강, 켜짐(신호 1 이상)은 밝은 빨강
- 분류 호퍼의 겉모습(태그 `v3`부터): 바닐라 호퍼 모양에 구리빛 테두리를 두르고 깔때기 바닥에 구리 거름망을 넣었다
  - 블록: 바닐라 호퍼보다 아주 조금 큰 모델이 호퍼를 덮는다. 대롱 방향(아래, 옆 네 방향)에 맞춰 돈다
  - 인벤토리 아이템: 거름망이 보이는 입구의 호퍼 그림
- 경험치 호퍼의 겉모습(태그 `v4`부터): 어두운 쇠 몸체에 연두빛 테두리와 청금석 띠를 둘렀고, 그릇 가운데에 빛나는 경험치 구슬이 떠 있다
  - 블록: 분류 호퍼와 같이 바닐라 호퍼를 덮고 대롱 방향에 맞춰 돈다
  - 인벤토리 아이템: 그릇 위로 경험치 구슬이 떠오른 호퍼 그림
- 총·탄·부착물의 겉모습(태그 `v5`부터): 실제 총의 생김새를 보고 직접 그린 평면 그림이다. 다른 제작자나 다른 게임의 그림·모델을 담지 않는다
  - 총 네 가지(32×32): Glock 17, Colt M4A1, Remington Model 870, Mosin-Nagant M91/30
  - 총 그림은 단 부착물(탄창, 총구, 조준기)에 따라 바뀐다. 조합마다 한 장씩 모두 71장이다
  - 개머리판은 그림에 보이지 않는다
  - 탄 열두 가지(16×16): 구경마다 모양이 다르다. 권총탄·소총탄은 탄두 끝 색(칠 없음, 초록, 검정)으로, 산탄은 껍데기 색(빨강, 파랑, 노랑)으로 단계를 나눈다
  - 부착물 열세 가지(16×16): 탄창 다섯, 소음기, 보정기, 초크, 개머리판 둘, 도트 조준기, 중거리 조준경, 저격 조준경
  - 총은 손에 들면 총구가 앞을 본다. 쏴서 남은 탄 수가 바뀌어도 손의 총이 다시 올라오지 않는다
  - 태그 `v6`: 손에 든 총의 방향을 고쳤다. `v5`에서는 1인칭에서 총구가 자기 쪽을 보고 3인칭에서 총이 뒤집혀 있었다. 이제 1인칭·3인칭 모두 총구가 앞을, 손잡이가 손을 본다. 인벤토리 그림은 그대로 총구가 오른쪽이다
- 총기 작업대의 겉모습(태그 `v5`부터): 어두운 쇠판 위에 총 모양 틀과 공구를 둔 블록이다
  - 옆면은 쇠 테두리를 두른 나무 서랍 두 칸, 앞면은 쇠 바이스와 공구걸이, 아랫면은 쇠 다리가 보이는 나무판이다
  - 블록과 인벤토리 아이템이 같은 모델을 쓴다
- 총소리(태그 `v7`부터): 녹음이나 다른 게임의 소리가 아니라 저장소의 스크립트로 직접 합성한 소리다
  - 총성 네 가지: Glock 17은 짧고 날카롭게, M4A1은 찢어지듯 단단하게, Remington 870은 깊게 쾅, Mosin-Nagant는 크게 터지고 길게 울린다
  - 총마다 소음기 총성이 따로 있고, 멀리 퍼지는 낮은 메아리가 한 가지 있다
  - 빈 총 딸깍, 걸림, 탄창 빼기·끼우기, 슬라이드, 펌프, 노리쇠 소리
  - 자막은 한국어와 영어다
  - 태그 `v8`: 걸림 소리를 뺀 총소리를 실제 총 녹음으로 바꿨다. 출처는 아래 "소리 출처"에 있다
- 바닐라 블록·아이템 그림은 바꾸지 않는다. 모든 파일은 `gameserver` 이름공간에만 있다

## 소리 출처
태그 `v8`부터 쓰는 녹음 17개다. 모두 Freesound에 CC0 1.0으로 올라온 것이다.

- Glock 19X: https://freesound.org/people/areniporgen/sounds/828786/ (올린 사람 areniporgen)
- Glock-G4.wav: https://freesound.org/people/hollandm/sounds/693357/ (올린 사람 hollandm)
- 9mm Pistol Gunshots: https://freesound.org/people/DledeSOUND/sounds/731942/ (올린 사람 DledeSOUND)
- Colt M4A1 SOCOM: https://freesound.org/people/areniporgen/sounds/737569/ (올린 사람 areniporgen)
- Saiga 12k Gunshot(12ga).mp3: https://freesound.org/people/Kobrakon47/sounds/569309/ (올린 사람 Kobrakon47)
- Sauer 404 close shot.wav: https://freesound.org/people/moosegravy/sounds/431834/ (올린 사람 moosegravy)
- 9MM suppressor: https://freesound.org/people/Biro2131/sounds/867604/ (올린 사람 Biro2131)
- Gunshot with silencer: https://freesound.org/people/hotpin7/sounds/819269/ (올린 사람 hotpin7)
- silenced pistol shot: https://freesound.org/people/Clutvh/sounds/627087/ (올린 사람 Clutvh)
- Distant Gunfire: https://freesound.org/people/iainmccurdy/sounds/842326/ (올린 사람 iainmccurdy)
- Dry Fire: https://freesound.org/people/brianhanson2nd/sounds/171211/ (올린 사람 brianhanson2nd)
- handgun-dryfire.wav: https://freesound.org/people/davdud101/sounds/119168/ (올린 사람 davdud101)
- Mag reload: https://freesound.org/people/SamsterBirdies/sounds/363167/ (올린 사람 SamsterBirdies)
- AR15 M4 Gun Hardware Magazine Movement Sounds: https://freesound.org/people/jackthemurray/sounds/393732/ (올린 사람 jackthemurray)
- Pump Action Shotgun: https://freesound.org/people/awrmacd/sounds/387190/ (올린 사람 awrmacd)
- Mosin Nagant Bolt Action Cycle: https://freesound.org/people/Zott820/sounds/370345/ (올린 사람 Zott820)
- Gun pull back 2: https://freesound.org/people/HyperFoley/sounds/789850/ (올린 사람 HyperFoley)

걸림 소리(`jam_1`, `jam_2`)는 맞는 녹음이 없어 직접 합성했다.

## 받기
릴리스의 `gameserver-resourcepack.zip`이 서버가 내려주는 파일이다. 태그마다 그림과 소리 한 벌이고, 이미 올린 태그의 파일은 바꾸지 않는다.

## 라이선스
이 팩의 텍스처와 모델은 이 서버를 위해 직접 만든 것이다. 총소리는 태그 `v8`부터 CC0 1.0 녹음(Freesound)을 잘라 다듬은 것이고, 걸림 소리만 직접 합성했다. 마인크래프트 원본 텍스처와 소리, 다른 게임의 소리를 담지 않는다.

Minecraft는 Mojang Studios의 상표이며, 이 팩은 Mojang Studios와 관계가 없다.
