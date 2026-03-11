<h1 align="center">LootExpansion</h1>

<p align="center">
  <img src="https://img.shields.io/badge/version-1.0.0-blue.svg?style=flat-square" alt="Version">
  <img src="https://img.shields.io/badge/game-MIMESIS-purple.svg?style=flat-square" alt="Game">
  <img src="https://img.shields.io/badge/MelonLoader-0.7.1%2B-green.svg?style=flat-square" alt="MelonLoader">
  <img src="https://img.shields.io/badge/status-working-brightgreen.svg?style=flat-square" alt="Status">
</p>

<p align="center">
  <strong>Mimesis</strong> 전용 고성능 동적 전리품 확장 시스템입니다.<br>
  실시간 환경 스캔을 통해 최적화된 드롭 테이블을 구성하고 협동 플레이의 가치를 높입니다.
</p>

<p align="center">
  <a href="#-english-version">🌐 <strong>Switch to English Version</strong></a>
</p>

---

## 📑 목차 (Contents)
1. [요구사항 (Requirements)](#1-요구사항-requirements)
2. [설치 방법 (Installation)](#2-설치-방법-installation)
3. [구성 (Configuration)](#3-구성-configuration)
4. [주요 특징 (Key Features)](#4-주요-특징-key-features)
5. [세부 설정 가이드 (Settings Guide)](#5-세부-설정-가이드-settings-guide)
6. [작동 방식 (How It Works)](#6-작동-방식-how-it-works)

---

## 1. 요구사항 (Requirements)
모드가 정상적으로 작동하기 위해 아래 라이브러리가 반드시 선행 설치되어야 합니다.
* **[MelonLoader v0.7.1+](https://melonwiki.xyz/)**
* **[MimicAPI](https://thunderstore.io/c/mimesis/p/NeoMimicry/MimicAPI/)** (Essential Dependency)

---

## 2. 설치 방법 (Installation)
1. **[Releases](https://github.com/xxxx-6666/2077-전리품-확장판/releases)** 페이지에서 최신 버전의 `LootExpansion.dll`을 다운로드합니다.
2. 게임 설치 경로 내 `MIMESIS/MelonLoader/Mods/` 폴더에 다운로드한 파일을 넣습니다.
3. 게임을 실행하여 모드가 정상적으로 로드되는지 확인합니다.

---

## 3. 구성 (Configuration)
첫 실행 후 생성되는 `UserData/MelonPreferences.cfg` 파일에서 상세 설정을 변경할 수 있습니다.

| Setting | Type | Default | Description |
| :--- | :--- | :--- | :--- |
| `Enabled` | `bool` | `true` | 모드 활성화 여부 |
| `Drop_Probability` | `float` | `1.0` | 아이템 드롭 확률 (0.1 ~ 1.0) |
| `Monster_Count` | `int` | `1 ~ 5` | 각 몬스터별 최대 드롭 수량 (0 ~ 10) |

---

## 4. 주요 특징 (Key Features)

### 확정 보상 및 밸런스 (Guaranteed Rewards & Balance)
* **Specific Drops**: 
    * **Ramblam**: 장전되지 않은 샷건과 탄약 1개를 드롭합니다.
    * **Heavy D**: 붐박스와 **금 목걸이**를 드롭합니다.
* **Exclusions**: 파밍 가치 보존을 위해 `Defective Bomb`, `Golden Statue`, `Shining Frog`는 드롭에서 제외됩니다.
* **Immersion**: 진짜와 가짜의 구분을 위해 `MIMIC` 및 `Bombesis`는 아이템을 드롭하지 않습니다.

---

## 5. 세부 설정 가이드 (Settings Guide)

`MelonPreferences.cfg`에서 조정 가능한 각 몬스터별 드롭 설정입니다.

| Key | Default | Description |
| :--- | :--- | :--- |
| `Sentryper_Count` | `5` | **센트리퍼** 처치 시 드롭 아이템 수 (최대 10) |
| `BruteBunny_Count` | `5` | **브루트 버니** 처치 시 드롭 아이템 수 (최대 10) |
| `Maegoostro_Count` | `3` | **매구스트로** 처치 시 드롭 아이템 수 (최대 10) |
| `StandingOwl_Count` | `1` | **스탠딩 아울** 처치 시 드롭 아이템 수 (최대 10) |
| `MrDelpit_Count` | `1` | **미스터 델핏** 처치 시 드롭 아이템 수 (최대 10) |
| `Quakka_Count` | `1` | **쿼카** 처치 시 드롭 아이템 수 (최대 10) |

---

## 6. 작동 방식 (How It Works)

### 스마트 구역 스캔 (Smart Area Scanning)
지역 진입(착륙) 후 **최초 5초간** 실내의 모든 전리품 데이터를 실시간으로 수집합니다. 이를 통해 현재 구역의 난이도와 테마에 가장 적합한 **동적 전리품 테이블**을 즉석에서 생성하여 적용합니다.

### 지능형 밸런스 알고리즘 (Intelligent Balancing)
몬스터의 행동 패턴, 반격 위험도, 그리고 체력을 종합적으로 분석하여 보상의 가치를 결정합니다. 위험을 감수하고 강력한 적을 처치한 팀에게 그에 걸맞은 높은 가치의 보상을 제공하도록 설계되었습니다.

<br>

---

# 🇺🇸 English Version

High-performance dynamic loot expansion system exclusively for **Mimesis**. It constructs optimized drop tables through real-time environment scanning and enhances the value of cooperative play.

## 📑 Contents
1. [Requirements](#1-requirements)
2. [Installation](#2-installation)
3. [Configuration](#3-configuration)
4. [Key Features](#4-key-features)
5. [Settings Guide](#5-settings-guide)
6. [How It Works](#6-how-it-works)

---

## 1. Requirements
The following libraries must be installed beforehand for the mod to function correctly.
* **[MelonLoader v0.7.1+](https://melonwiki.xyz/)**
* **[MimicAPI](https://thunderstore.io/c/mimesis/p/NeoMimicry/MimicAPI/)** (Essential Dependency)

---

## 2. Installation
1. Download the latest `LootExpansion.dll` from the **[Releases](https://github.com/xxxx-6666/2077-전리품-확장판/releases)** page.
2. Place the downloaded file in the `MIMESIS/MelonLoader/Mods/` folder within your game installation path.
3. Launch the game and verify that the mod is loaded correctly.

---

## 3. Configuration
Detailed settings can be modified in the `UserData/MelonPreferences.cfg` file generated after the first run.

| Setting | Type | Default | Description |
| :--- | :--- | :--- | :--- |
| `Enabled` | `bool` | `true` | Toggle mod functionality |
| `Drop_Probability` | `float` | `1.0` | Item drop chance (0.1 ~ 1.0) |
| `Monster_Count` | `int` | `1 ~ 5` | Max drop quantity per monster (0 ~ 10) |

---

## 4. Key Features

### Guaranteed Rewards & Balance
* **Specific Drops**: 
    * **Ramblam**: Drops an unloaded shotgun and 1 ammo.
    * **Heavy D**: Drops a boombox and a **Gold Necklace**.
* **Exclusions**: To preserve farming value, `Defective Bomb`, `Golden Statue`, and `Shining Frog` are excluded from drops.
* **Immersion**: To distinguish between real and fake, `MIMIC` and `Bombesis` do not drop items.

---

## 5. Settings Guide

Detailed drop settings for each monster adjustable in `MelonPreferences.cfg`.

| Key | Default | Description |
| :--- | :--- | :--- |
| `Sentryper_Count` | `5` | Drop count for **Sentryper** (Max 10) |
| `BruteBunny_Count` | `5` | Drop count for **BruteBunny** (Max 10) |
| `Maegoostro_Count` | `3` | Drop count for **Maegoostro** (Max 10) |
| `StandingOwl_Count` | `1` | Drop count for **StandingOwl** (Max 10) |
| `MrDelpit_Count` | `1` | Drop count for **MrDelpit** (Max 10) |
| `Quakka_Count` | `1` | Drop count for **Quakka** (Max 10) |

---

## 6. How It Works

### Smart Area Scanning
Collects real-time loot data from all interiors for the **first 5 seconds** after entering an area (landing). Based on this, it generates and applies a **dynamic loot table** most suitable for the current area's difficulty and theme on the fly.

### Intelligent Balancing Algorithm
Determines the value of rewards by comprehensively analyzing the monster's behavior patterns, counterattack risk, and health. It is designed to provide rewards worthy of the effort to teams that take risks to defeat powerful enemies.

---

> [!TIP]
> **Need help?** Visit our [Official Discord Server](https://github.com/xxxx-6666/2077-전리품-확장판) for fast technical support and configuration assistance!

<p align="center">
  Developed with ❤️ by <strong>GOXH</strong><br>
  © 2026 LootExpansion. All rights reserved.
</p>
