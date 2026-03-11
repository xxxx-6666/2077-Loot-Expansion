# LootExpansion

**MelonLoader 0.7.1** 기반으로 제작된 **Mimesis** 전용 고성능 전리품 확장 모드입니다. 

이 모드는 지역 진입 시 주변 환경을 스캔하여 **동적 전리품 테이블**을 생성하며, 몬스터가 현재 위치에 적합한 아이템을 드롭하도록 보장합니다. 더욱더 파밍이 재밌고, 팀원들과 협동하여 위험의 고비를 넘기면 그에 따른 확실한 보상을 제공하는 것이 특징입니다.

## 필수 요구 사항
이 모드가 작동하려면 **[MimicAPI](https://thunderstore.io/c/mimesis/p/NeoMimicry/MimicAPI/)**가 반드시 필요합니다. 모드를 실행하기 전에 MimicAPI가 설치되어 있는지 확인해 주세요.

## 주요 기능
* **몬스터 전용 확정 드롭**: 
    * **Ramblam**: 장전되지 않은 샷건과 샷건 탄약 1개를 드롭합니다.
    * **Heavy D**: 붐박스와 **금 목걸이**를 드롭합니다.
* **파밍 밸런스 유지 (특수 아이템 제외)**: 파밍의 목적성을 명확히 하기 위해 아래 아이템들은 몬스터 드롭 테이블에서 제외되었습니다.
    * **제외 아이템**: Defective Bomb, Golden Statue, Shining Frog
* **몰입형 논-드롭 시스템**: **MIMIC** 및 **Bombesis**는 가짜 아이템을 드롭하기 때문에, 진짜와 가짜의 구분이 어려운 몰입감을 위해 아이템을 드롭하지 않습니다.
* **지능형 밸런스 적용**: 그 외 몬스터들은 행동, 반격, 체력을 고려하여 드롭되는 아이템들의 가격 가중치 밸런스가 적용되었습니다.
* **커스텀 드롭 수량**: 몬스터에 따라서 드롭할 수 있는 아이템 개수를 최소 0개에서 최대 10개까지 설정 가능합니다.
* **스마트 구역 스캔**: 착륙 후 5초 동안 자동으로 실내 전리품 데이터를 수집합니다.
* **최적화된 클린 코드**: 불필요한 변수와 메서드를 제거하여 FPS 안정성을 극대화했습니다.
* **자동 초기화 시스템**: 지역 이동 시 모든 캐시를 초기화하여 메모리 누수와 전리품 중복을 방지합니다.

## 모드 설정 (Configuration)
게임 실행 후 생성되는 `UserData/MelonPreferences.cfg` 파일에서 아래 항목들을 수정할 수 있습니다. 
**설정법을 잘 모르시겠다면 저희 디스코드 서버를 방문해주세요!**

* **Enabled**: 모드 활성화 여부 (True/False)
* **Drop_Probability**: 드롭 확률 (0.1 = 10% / 1.0 = 100%)
* **몬스터별 드롭 개수 설정 (범위: 0~10)**:
    1. **Sentryper_Count**: Sentryper 처치 시 드롭 아이템 수
    2. **BruteBunny_Count**: BruteBunny 처치 시 드롭 아이템 수
    3. **Maegoostro_Count**: Maegoostro 처치 시 드롭 아이템 수
    4. **StandingOwl_Count**: StandingOwl 처치 시 드롭 아이템 수
    5. **MrDelpit_Count**: MrDelpit 처치 시 드롭 아이템 수
    6. **Quakka_Count**: Quakka 처치 시 드롭 아이템 수

## 설치 방법
1. [MelonLoader v0.7.1+](https://melonwiki.xyz/)를 설치합니다.
2. [MimicAPI](https://thunderstore.io/c/mimesis/p/NeoMimicry/MimicAPI/)를 설치합니다.
3. [GitHub](https://github.com/xxxx-6666)에서 최신 릴리즈를 다운로드합니다.
4. `LootExpansion.dll` 파일을 게임 경로의 `Mimesis/Mods` 폴더에 넣습니다.

## 상세 사양
* **게임 버전**: Mimesis v0.2.8+
* **프레임워크**: MelonLoader v0.7.2+
* **선행 모드**: MimicAPI

---

# LootExpansion (English)

A high-performance loot expansion mod for **Mimesis**, built on **MelonLoader 0.7.1**.

This mod scans the environment upon entering an area to generate **dynamic loot tables**, ensuring that monsters drop items appropriate for their current location. It enhances the farming experience by rewarding players for overcoming high-risk situations through teamwork.

## Requirements
This mod requires **[MimicAPI](https://thunderstore.io/c/mimesis/p/NeoMimicry/MimicAPI/)** to function. Please ensure MimicAPI is installed before running the mod.

## Key Features
* **Guaranteed Monster Drops**:
    * **Ramblam**: Drops an unloaded shotgun and 1 shotgun shell.
    * **Heavy D**: Drops a boombox and a **Gold Necklace**.
* **Loot Balance Integrity**: To ensure a clear sense of progression and farming goals, the following items are excluded from monster drop tables:
    * **Excluded Items**: Defective Bomb, Golden Statue, Shining Frog
* **Immersive Non-Drop System**: To maintain the challenge of distinguishing real items from fakes, **MIMIC** and **Bombesis** do not drop items upon death.
* **Intelligent Balance Algorithm**: For all other monsters, loot drops are balanced based on their behavior, counter-attack risk, and health.
* **Custom Drop Count**: Configure the number of items dropped per monster, ranging from **0 to 10**.
* **Smart Area Scanning**: Automatically collects indoor loot data for 5 seconds after landing.
* **Performance Optimized**: Clean code architecture with minimal overhead to ensure maximum FPS stability.
* **Auto-Reset System**: Clears all caches when moving to a new area to prevent memory leaks and loot duplication.

## Configuration
Settings can be adjusted in the `UserData/MelonPreferences.cfg` file after the first run.
**If you are unsure how to configure the settings, please visit our Discord server!**

* **Enabled**: Toggle Mod Activation (True/False)
* **Drop_Probability**: Drop chance (0.1 = 10% / 1.0 = 100%)
* **Per-Monster Drop Count (Range: 0-10)**:
    1. **Sentryper_Count**: Number of items dropped by Sentryper
    2. **BruteBunny_Count**: Number of items dropped by BruteBunny
    3. **Maegoostro_Count**: Number of items dropped by Maegoostro
    4. **StandingOwl_Count**: Number of items dropped by StandingOwl
    5. **MrDelpit_Count**: Number of items dropped by MrDelpit
    6. **Quakka_Count**: Number of items dropped by Quakka

## Installation
1. Install [MelonLoader v0.7.1+](https://melonwiki.xyz/).
2. Install [MimicAPI](https://thunderstore.io/c/mimesis/p/NeoMimicry/MimicAPI/).
3. Download the latest release from [GitHub](https://github.com/xxxx-6666).
4. Place `LootExpansion.dll` into the `Mimesis/Mods` folder.

## Specifications
* **Game Version**: Mimesis v0.2.8+
* **Framework**: MelonLoader v0.7.2+
* **Dependency**: MimicAPI
