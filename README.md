# 팀 프로젝트 - 코코두기

<div align="center">
  <img width="1080" height="auto" alt="Image" src="README/Title.jpg" />
</div>


---


## 게임 소개

"모험심 강한 강아지, 코코두기의 집으로 돌아가는 여정기."

스테이지 별로 존재하는 맵의 기믹을 파악하고, 최소한의 행동력을 소모해서 집을 돌아가는 길찾기 퍼즐게임입니다.


---


## 🎮 프로젝트 개요

| 항목 | 내용 |
| ------ | ------ |
| **프로젝트명** | 코코두기 |
| **개발 기간** | 2025.10. ~ 2025.12. |
| **개발 인원** | 기획 4인, 개발 6인 |
| **개발 엔진** | Unity 6000.1 Support |
| **개발 언어** | C# |
| **타겟 플랫폼** | Android |


---


## Command Pattern 플로우

<div align="center">
  <img width="1080" height="auto" alt="Image" src="README/CommandUse.png" />
</div>


---


## 주요 기능

### 맵 에디터
* 게임 내에서 사용될 맵 에디터를 만들기 위한 시스템
* 맵 데이터는 json 규격으로 작성됨

> #### 관련 스크립트 및 폴더 링크
> * [**MapEditor/Scripts**](https://github.com/Sirosi/CocoDoogy/blob/main/Assets/_MapEditor/Scripts)
> * [MapEditorController.cs](https://github.com/Sirosi/CocoDoogy/blob/main/Assets/_MapEditor/Scripts/Controller/MapEditorController.cs)
> * [MapSaveLoader.cs](https://github.com/Sirosi/CocoDoogy/blob/main/Assets/_Project/Scripts/Utility/MapSaveLoader.cs)


<br/>


### 파이어베이스 연동
* Firebase의 기능을 사용하기 위한 시스템

> #### 관련 스크립트 및 폴더 링크
> * [**Network**](https://github.com/Sirosi/CocoDoogy/blob/main/Assets/_Project/Scripts/Network)
> * [FirebaseManager.cs](https://github.com/Sirosi/CocoDoogy/blob/main/Assets/_Project/Scripts/Network/FirebaseManager.cs)


<br/>


### 인게임 처리
* 플레이어의 행동 및 시스템의 행동을 동작/기록
* 플레이어 행동 이후에 시스템 처리를 위한 로직 처리

> #### 관련 스크립트 및 폴더 링크
> * [**GameFlow/InGame**](https://github.com/Sirosi/CocoDoogy/tree/main/Assets/_Project/Scripts/GameFlow/InGame)
> * [**GameFlow/InGame/Phase**](https://github.com/Sirosi/CocoDoogy/tree/main/Assets/_Project/Scripts/GameFlow/InGame/Phase)
> * [InGameManager.cs](https://github.com/Sirosi/CocoDoogy/blob/main/Assets/_Project/Scripts/GameFlow/InGame/InGameManager.cs)
> * [PlayerHandler.cs](https://github.com/Sirosi/CocoDoogy/blob/main/Assets/_Project/Scripts/GameFlow/InGame/PlayerHandler.cs)
> * [**GameFlow/InGame/Command**](https://github.com/Sirosi/CocoDoogy/tree/main/Assets/_Project/Scripts/GameFlow/InGame/Command)
> * [CommandManager.cs](https://github.com/Sirosi/CocoDoogy/blob/main/Assets/_Project/Scripts/GameFlow/InGame/Command/CommandManager.cs)


<br/>


### 타일 및 기물 시스템
* 타일은 게임의 맵을 구성하는 기본 요소
* 기물은 타일 위에 올라가는 요소

> #### 관련 스크립트 및 폴더 링크
> * [**Tile**](https://github.com/Sirosi/CocoDoogy/tree/main/Assets/_Project/Scripts/Tile)
> * [HexTile.cs](https://github.com/Sirosi/CocoDoogy/blob/main/Assets/_Project/Scripts/Tile/HexTile.cs)
> * [HexTileMap.cs](https://github.com/Sirosi/CocoDoogy/blob/main/Assets/_Project/Scripts/Tile/HexTileMap.cs)
> * [**Tile/Piece**](https://github.com/Sirosi/CocoDoogy/tree/main/Assets/_Project/Scripts/Tile/Piece)
> * [Piece.cs](https://github.com/Sirosi/CocoDoogy/blob/main/Assets/_Project/Scripts/Tile/Piece/Piece.cs)
> * [BridgePiece.cs](https://github.com/Sirosi/CocoDoogy/blob/main/Assets/_Project/Scripts/Tile/Piece/BridgePiece.cs)


<br/>


### 기믹 시스템
* 인게임에서 타일의 회전, 기물 변경 등을 동작시키는 시스템

> #### 관련 스크립트 링크
> * [GimmickExecutor.cs](https://github.com/Sirosi/CocoDoogy/blob/main/Assets/_Project/Scripts/Tile/Gimmick/GimmickExecutor.cs)
> * [GimmickData.cs](https://github.com/Sirosi/CocoDoogy/blob/main/Assets/_Project/Scripts/Tile/Gimmick/Data/GimmickData.cs)
> * [LeverPiece.cs](https://github.com/Sirosi/CocoDoogy/blob/main/Assets/_Project/Scripts/Tile/Piece/Trigger/LeverPiece.cs)


---


<br/>


## Thrid Party Library

<div align="center">
  <img width="auto" height="200" alt="Image" src="README/Firebase.png" />
  <img width="auto" height="200" alt="Image" src="README/FMOD.png" />
</div>