# OLED 실험 6주차 — Exciplex

**작성자:** 이영빈 **학번:** 2023101942

> 측정 시료: **m-MTDATA(전자주개, donor) / BPhen(전자받개, acceptor) / m-MTDATA:BPhen(1:1, exciplex)**
> 측정: UV–Vis 흡수(absorption), 광발광(photoluminescence, PL, λex = 280 nm)

---

## Ⅰ. 실험 목적

- 전자주개(electron donor)와 전자받개(electron acceptor) 두 이종 유기물이 계면에서 만나거나 혼합될 때 형성되는 **charge-transfer(CT) 상태**와 그에 따른 **exciplex 발광**을 이해한다.
- m-MTDATA와 BPhen 각각의 단일 박막, 그리고 두 물질을 혼합한 박막의 흡수·발광 스펙트럼을 측정·비교하여 exciplex 생성을 실험적으로 확인한다.
- Exciplex 발광 peak의 λmax·모양을 단일 물질과 비교하고, exciplex의 발광 에너지가 HOMO(donor)–LUMO(acceptor) 차이로 설명되는지 검증한다.
- 열증착 공정에서 **tooling factor**의 의미를 이해하고, 목표 두께와 실제 두께의 비로부터 보정 tooling factor를 산출한다.

---

## Ⅱ. 실험 원리

### A. Donor–Acceptor와 charge-transfer complex

유기 반도체에는 전자를 내주기 쉬운 **donor**(보통 정공수송재료, 얕은 HOMO)와 전자를 받기 쉬운 **acceptor**(보통 전자수송재료, 깊은 LUMO)가 있다. 이 둘이 접촉하면 경계에서 donor의 HOMO에 있던 전자가 acceptor의 LUMO 쪽으로 부분적으로 이동한 **부분 전하이동(partial charge transfer) 상태**가 만들어진다. 이렇게 두 분자가 한 쌍처럼 거동하며 새로운 광학적 특성을 보이는 상태를 charge-transfer complex라 하며, 이때 단일 물질에 없던 새로운 흡수(CT absorption)나 발광(exciplex emission)이 나타난다.

### B. Exciplex vs excimer

- **Excimer**: 들뜬 분자가 **같은 종류**의 바닥상태 분자와 결합하여 형성되는 들뜬 이합체.
- **Exciplex(excited complex)**: **서로 다른 종류**(donor·acceptor)의 분자 사이에서 형성되는 들뜬 상태 복합체.

Exciplex emission의 특징은 (ⅰ) 단일 물질보다 **장파장(저에너지)** 에서 나타나고, (ⅱ) **broad**하며, (ⅲ) **진동 구조(vibrational/vibronic structure)가 없는** 매끄러운 single peak라는 점이다. 이는 CT 상태가 공유결합이 아닌 느슨한 쿨롱 상호작용으로 묶인 상태라 뚜렷한 진동 모드를 갖지 않고, donor·acceptor보다 안정한(에너지가 낮은) 새 상태를 만들기 때문이다.

### C. Exciplex 발광 에너지와 HOMO–LUMO

Exciplex의 발광 에너지는 근사적으로 donor의 HOMO와 acceptor의 LUMO 사이의 에너지 차(CT gap)로 설명된다.

```
h·ν(exciplex) ≈ | E_HOMO(donor) − E_LUMO(acceptor) | − (쿨롱 결합에너지 등 보정항)
```

따라서 발광 λmax를 에너지로 환산(E = 1240/λ[nm])하여 HOMO(D)−LUMO(A) 값과 비교하면 exciplex 형성 여부와 CT 특성을 판정할 수 있다.

### D. Tooling factor (열증착 두께 보정)

열증착기에서 두께는 **QCM(quartz crystal microbalance)** 센서가 측정하는데, 센서는 기판과 다른 위치에 있으므로 실제 기판 증착량과 차이가 난다. 이 기하학적 차이를 보정하는 비례상수가 tooling factor다.

```
보정 tooling factor = 초기 tooling factor × (실제 측정 두께 / 목표(설정) 두께)
```

---

## Ⅲ. 실험 방법

### A. 기구 및 재료

| 구분 | 항목 |
|------|------|
| 측정 장비 | Photoluminescence spectrometer(JASCO FP-8550), UV/VIS spectrophotometer(JASCO V-750), Thermal evaporator, Alpha-step(두께 측정) |
| 시료 | m-MTDATA(donor), BPhen(acceptor), bare glass(기판) |

### B. 실험 과정

1. donor(m-MTDATA)와 acceptor(BPhen)를 준비한다.
2. thermal evaporator로 증착한 뒤 실제 두께를 측정하여 **tooling factor**를 구한다.
3. m-MTDATA 단일 박막, BPhen 단일 박막을 각각 제작한다.
4. m-MTDATA:BPhen = 1:1 혼합(공증착) 박막을 제작한다.
5. 3종 박막의 **absorption**과 **photoluminescence(λex = 280 nm)** 를 측정한다.
6. 각 스펙트럼의 peak 파장을 비교하여 exciplex 생성을 확인한다.

---

## Ⅳ. 실험 결과 (Result)

### 1. 박막 두께 측정 및 tooling factor

- 초기 tooling factor = **23.7 %**
- 목표(설정) 두께 = **800 Å**
- 실제 측정 두께 = **600 Å**

```
보정 tooling factor = 23.7 × (600 / 800)
                    = 23.7 × 0.75
                    = 17.775 ≈ 17.8 %
```

실제 두께(600 Å)가 목표(800 Å)보다 작게 증착되었으므로, 센서가 과대평가하고 있었다는 뜻이다. tooling factor를 **17.8 %로 낮춰** 다음 증착부터 센서 두께와 실제 두께가 일치하도록 보정한다.

### 2. Exciplex PL spectrum의 λmax와 peak 모양 비교

**Fig. 1 — 3종 박막의 PL 스펙트럼 (정규화, λex = 280 nm)**

![PL overlay](figures/fig_pl_overlay.png)

**Fig. 2 — 3종 박막의 PL 스펙트럼 (원시 강도)**

![PL raw](figures/fig_pl_raw.png)

| 시료 | PL λmax | FWHM(반치폭) | peak 모양 |
|------|:-------:|:-----------:|-----------|
| m-MTDATA (donor) | **428 nm** | 약 46 nm | 비교적 좁고 단일 |
| BPhen (acceptor) | **396 nm** | 약 81 nm | 넓은 편 |
| **m-MTDATA:BPhen (exciplex)** | **538 nm** | 약 89 nm | 매우 broad, 진동 구조 없는 매끄러운 single peak |

**해석.** 혼합 박막의 PL peak(538 nm)는 단일 물질(m-MTDATA 428 nm, BPhen 396 nm)에 비해 **약 110~140 nm 장파장(저에너지)으로 크게 이동**했고, FWHM도 가장 넓다. 또한 단일 물질 발광의 단순 합(중첩)으로는 설명되지 않는 **새로운 peak**가 장파장에 나타났다. 이는 두 단일 물질 어디에도 없던 새로운 발광종, 즉 **exciplex(CT 상태) emission**이 생성되었음을 뜻한다. 진동 구조가 보이지 않고 매끄러운 것도 exciplex의 전형적 특징과 일치한다.

### 3. Exciplex의 band gap과 HOMO(Donor)–LUMO(Acceptor) 비교

**Fig. 3 — 3종 박막의 UV–Vis 흡수 스펙트럼**

![ABS overlay](figures/fig_abs_overlay.png)

**Fig. 4 — Exciplex의 charge-transfer 에너지 다이어그램**

![energy diagram](figures/fig_energy_ct.png)

- Exciplex PL λmax = 538 nm → 발광 에너지 **E = 1240 / 538 ≈ 2.30 eV**
- 문헌 에너지 준위(근사): **HOMO(m-MTDATA) ≈ -5.1 eV**, **LUMO(BPhen) ≈ -2.6 eV**
- 기대 CT gap = |−5.1 − (−2.6)| = **2.5 eV** → 파장 환산 약 496 nm

| 항목 | 값 |
|------|------|
| Exciplex 발광 에너지 (PL λmax 538 nm) | 약 2.30 eV |
| HOMO(D) − LUMO(A) 기대값 | 약 2.50 eV |
| 혼합 박막 흡수 onset | 약 431 nm → 2.88 eV |

**해석.** 실험으로 얻은 exciplex 발광 에너지(≈ 2.30 eV)는 HOMO(D)−LUMO(A)로 예상되는 CT gap(≈ 2.50 eV)과 같은 수준(차이 약 0.2 eV)으로 잘 대응한다. 발광 에너지가 CT gap보다 약간 낮은 것은 exciplex가 형성 후 CT 상태의 쿨롱 안정화 에너지와 구조 완화(relaxation)만큼 더 낮은 에너지에서 발광하기 때문이며, 이는 exciplex 발광이 단순 단분자 발광이 아니라 **donor–acceptor 간 전하이동 발광**임을 뒷받침한다. 흡수 onset(2.88 eV)이 발광 에너지(2.30 eV)보다 큰 것(큰 Stokes shift)도 CT 발광의 특징이다.

### 4. TADF 물질과 exciplex의 차이 (지침서 결과 4번)

| 구분 | TADF 단분자 | Exciplex |
|------|-------------|----------|
| CT 상태 위치 | **한 분자 내** D–A 단위 | **두 분자 사이**(intermolecular) |
| ΔE(S₁–T₁) | 매우 작게 분자 설계로 구현 | 공간 분리로 자연히 매우 작음 |
| 발광 스펙트럼 | 비교적 좁음 | 매우 broad, 구조 없음 |
| 제어성 | 분자 구조로 색 조절 | D/A 조합·혼합비로 조절 |

자세한 비교는 Ⅴ. 고찰 3번에서 서술한다.

---

## Ⅴ. 고찰 (Discussion)

### 1. QCM 센서에 대한 설명

QCM(Quartz Crystal Microbalance, 수정진동자 미량저울)은 **AT-cut 수정 결정의 공진 주파수가 표면에 쌓인 질량에 따라 감소**하는 성질을 이용한 질량 센서다. 수정에 교류 전압을 걸면 역압전 효과로 고유 공진 주파수(수 MHz)로 진동하는데, 증착 물질이 결정 표면에 쌓이면 유효 질량이 늘어 공진 주파수가 낮아진다. 얇은 강체 막에서는 **Sauerbrey 식**에 따라 주파수 변화가 단위면적당 질량 변화에 선형 비례한다.

```
Δf = − (2 f₀² / (A·√(ρq·μq))) · Δm
```

증착기는 이 Δf로부터 센서 위치의 증착 두께를 실시간 계산한다. 다만 센서는 기판과 다른 위치·각도에 있어 실제 기판 두께와 차이가 생기므로, **tooling factor로 보정**해 센서 지시값을 실제 기판 두께에 맞춘다. 본 실험의 tooling 보정(23.7 → 17.8 %)이 바로 이 과정이다.

### 2. Exciplex 발광에 vibrational peak이 뚜렷하지 않은 이유

단분자 발광에서는 전자 전이가 특정 진동 준위들로 떨어지며 여러 개의 **vibronic(진동-전자) peak**(피크가 어깨처럼 겹쳐 나타남)을 만든다. 그러나 exciplex의 발광은 donor의 HOMO와 acceptor의 LUMO 사이의 **전하이동(CT) 전이**로, 발광종이 공유결합으로 단단히 묶인 하나의 분자가 아니라 **두 분자가 느슨하게 쿨롱 상호작용으로 결합한 상태**이다. 이 상태는

- 잘 정의된 분자 진동 모드를 갖지 않고,
- donor–acceptor 간 거리·배향이 연속적으로 분포하여 발광 에너지가 넓게 퍼지며,
- 주변 환경(분극)에 의한 요동이 커

진동 구조가 평탄화(smearing)된다. 그 결과 exciplex PL은 날카로운 vibronic peak 없이 **broad하고 매끄러운 single Gaussian형 peak**로 나타난다. 실제 Fig. 1에서 exciplex(538 nm) 곡선은 단일 물질보다 넓고 구조가 없는 매끄러운 형태를 보였다.

### 3. Exciplex의 지연발광(delayed emission) 가능 이유 및 TADF와의 차이

**지연발광이 가능한 이유.** Exciplex에서는 전자(acceptor LUMO)와 정공(donor HOMO)이 **공간적으로 서로 다른 분자에 분리**되어 있다. 이 공간 분리는 교환 상호작용(exchange interaction)을 작게 만들어 **singlet CT 상태와 triplet CT 상태의 에너지 차 ΔE(S₁–T₁)를 매우 작게**(수십 meV 이하) 만든다. ΔE가 열에너지(상온 kT ≈ 26 meV) 수준으로 작으면, 삼중항(T₁)에 갇힌 여기자가 열적으로 다시 일중항(S₁)으로 **역계간전이(RISC, reverse intersystem crossing)** 할 수 있고, 이후 S₁ → S₀로 발광한다. 이 경로가 즉시발광(prompt)보다 시간이 걸리므로 **지연형광(delayed fluorescence)** 으로 관측된다. 즉 exciplex는 그 자체로 **TADF(열활성 지연형광) 메커니즘**을 보일 수 있다.

**TADF 물질과 exciplex의 차이.**

- **CT 상태의 공간 규모.** TADF 단분자는 하나의 분자 안에 donor·acceptor 단위를 붙여 **분자 내(intramolecular) CT**를 만든다. Exciplex는 **서로 다른 두 분자 사이(intermolecular)** 의 CT다.
- **ΔE(S₁–T₁) 확보 방식.** TADF는 donor/acceptor를 비틀어(dihedral twist) HOMO–LUMO 공간 중첩을 줄이는 정교한 분자 설계로 작은 ΔE를 얻는다. Exciplex는 두 분자가 떨어져 있어 **본질적으로** 작은 ΔE를 갖는다.
- **스펙트럼·효율.** Exciplex 발광은 TADF 단분자보다 더 broad하고, 농도·혼합비·형태에 민감하여 색 재현성과 효율 제어가 상대적으로 어렵다. 반면 조성만 바꿔 쉽게 발광색을 조절할 수 있다는 장점도 있다.
- **응용.** 둘 다 삼중항 여기자를 활용해 내부 양자효율 100%에 근접할 수 있으나, exciplex는 주로 **host나 보조 발광/전하 균형층**으로, TADF 단분자는 **발광 도판트**로 많이 쓰인다.

---

### 부록 — 데이터 처리 요약

- 측정 기기: PL(JASCO FP-8550, λex 280 nm, 300–800 nm), UV–Vis(JASCO V-750, 250–500 nm)
- λmax: PL 스펙트럼에서 330 nm 이상 영역의 최대 강도 파장
- FWHM: 최대 강도의 절반 높이에서 좌/우 교차점을 선형 보간하여 산출
- exciplex 흡수 onset: 흡수 상승 edge의 선형회귀와 장파장 baseline의 교점
- 에너지 환산: E[eV] = 1240 / λ[nm]
- 모든 그래프는 측정 raw CSV로부터 Python(numpy/matplotlib)으로 직접 작성
- 문헌 에너지 준위(m-MTDATA HOMO ≈ -5.1 eV, BPhen LUMO ≈ -2.6 eV)는 근사 비교용 참고값
