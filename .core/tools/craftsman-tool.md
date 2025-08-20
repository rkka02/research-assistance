# craftsman-tool.md
# 츠구미의 정밀 도구함 - Precision Optics & Holography Implementation Tools

## Digital Holography & Interferometry Tools

### Holographic Interferometry Systems
**Digital Holographic Reconstruction Framework**
```python
class DigitalHolographyProcessor:
    def __init__(self, wavelength=632.8e-9, pixel_size=5.2e-6):
        self.wavelength = wavelength
        self.pixel_size = pixel_size
        self.reconstruction_distance = None
    
    def reconstruct_hologram(self, hologram, reference_wave):
        """
        디지털 홀로그램에서 3D 객체 재구성
        머신러닝 기반 초해상도 기법 적용
        """
        # Fresnel 변환을 통한 홀로그램 재구성
        # 위상 언래핑과 노이즈 제거
        return reconstructed_amplitude, reconstructed_phase
```

**Quantitative Phase Imaging (QPI)**
- 위상 정보에서 물리적 특성 정밀 추출
- 나노미터 수준 두께 변화 측정
- 실시간 변형 모니터링
- 3D 형태학적 분석과 부피 측정

### Laser Interferometry Precision
**Michelson-Morley Type Interferometers**
- 피코미터(10⁻¹²m) 수준 변위 측정 달성
- 중력파 검출 수준 정밀도 (LIGO: 10⁻¹⁸m)
- 레이저 주파수 안정화 ±1 Hz in 10¹⁴ Hz
- 능동 진동 격리와 열적 안정성 제어

**Fabry-Perot Cavity Stabilization**
```python
def laser_frequency_stabilization(cavity_length, target_finesse=100000):
    """
    Pound-Drever-Hall 기법을 이용한 레이저 주파수 안정화
    cavity_length: 공진기 길이 (m)
    target_finesse: 목표 finesse 값
    """
    # 오차 신호 생성과 피드백 제어
    # 압전 소자를 통한 실시간 길이 보정
    return stabilized_frequency, error_signal
```

## Optical Coherence & Wavefront Control

### Coherence Length Optimization
**Temporal Coherence Management**
- 레이저 라인 폭 최소화 (<1 kHz)
- 모드-락 레이저를 통한 펄스 안정화
- 위상 잠금 루프 (PLL) 구현
- 클럭 지터 10⁻¹⁵ 수준 달성

**Spatial Coherence Enhancement**
- 단일 모드 광섬유를 통한 공간 필터링
- 가우시안 빔 프로파일 최적화
- M² 파라미터 1.05 미만 달성
- 빔 포인팅 안정성 ±0.1 μrad

### Adaptive Optics Implementation
**Wavefront Sensing Systems**
- Shack-Hartmann 센서를 통한 실시간 파면 측정
- 변형 미러 (DM)를 이용한 파면 보정
- 1000Hz 이상 폐루프 대역폭 달성
- Strehl ratio 0.9 이상 유지

**Atmospheric Turbulence Compensation**
```python
class AdaptiveOpticsController:
    def __init__(self, actuator_count=97, sampling_rate=2000):
        self.actuators = actuator_count
        self.loop_freq = sampling_rate
        self.control_matrix = None
    
    def correct_wavefront(self, wavefront_sensor_data):
        """
        실시간 파면 보정 알고리즘
        Zernike 다항식 기반 파면 분해
        """
        # 파면 기울기 계산과 제어 신호 생성
        return corrected_wavefront, residual_error
```

## Universal Measurement Uncertainty Framework

### JCGM 100:2008 Standard Implementation
**Type A/B Uncertainty Evaluation**
- 통계적 분석을 통한 Type A 불확실성
- 과학적 판단 기반 Type B 불확실성
- 합성 표준 불확실성 계산
- 확장 불확실성과 포함 인자 적용

**Monte Carlo Error Propagation**
```python
def optical_measurement_uncertainty(measured_values, systematic_errors):
    """
    광학 측정에서 불확실성 전파
    coherence length, wavelength stability, detector noise 고려
    """
    # 무작위 샘플링을 통한 불확실성 전파
    # 비선형 광학 효과의 불확실성 포함
    return measurement_result, expanded_uncertainty
```

## Systematic Error Control Systems

### Environmental Effect Monitoring
**온도 제어 시스템**
- ±0.01°C 수준 온도 안정화
- 다중 지점 온도 모니터링
- 온도 구배 영향 평가 및 보정
- 열팽창 계수를 고려한 교정

**Vibration Isolation**
- 수동 시스템: 스프링과 댐퍼 조합
- 능동 시스템: 지진 감지기와 모터 피드백
- 4중 진자 시스템 (LIGO 스타일)
- 1Hz 미만 주파수에서 10⁻¹⁰ 수준 격리

**Electromagnetic Interference (EMI) Control**
- Faraday 케이지 설계와 구현
- 접지 시스템과 차폐 효과성
- 필터링과 신호 무결성 보장
- RF 간섭 최소화 기법

### Instrumental Calibration Protocols
**Multi-Point Calibration**
- 전체 측정 범위에 걸친 교정점 설정
- 비선형성 검출과 보정 함수 개발
- 교정 곡선의 불확실성 평가
- 표준 참조 물질과의 추적성 확보

**Drift Monitoring & Correction**
- 장기간 안정성 추적
- Check standards를 이용한 일일 검증
- 자동 재교정 트리거 설정
- 드리프트 보정 알고리즘 적용

## Quality Management Systems

### Statistical Process Control (SPC)
**Control Charts Implementation**
```python
class LeveyJenningsChart:
    def __init__(self, target_value, std_dev):
        self.target = target_value
        self.warning_limits = (target_value ± 2*std_dev)
        self.control_limits = (target_value ± 3*std_dev)
    
    def check_westgard_rules(self, data_points):
        """
        Westgard 다중 규칙 적용:
        1₂s, 1₃s, 2₂s, R₄s, 4₁s, 10x̄
        """
        return rule_violations
```

**Quality Metrics Tracking**
- 측정 능력 지수 (Cp, Cpk) 계산
- 공정 성능 지수 (Pp, Ppk) 모니터링
- Six Sigma 품질 수준 달성
- 결함률 추적과 개선 목표 설정

### Round Robin Testing
**Inter-laboratory Comparison**
- 표준 시료를 이용한 실험실 간 비교
- Z-score 기반 성능 평가
- 편향 감지와 이상값 식별
- ISO/IEC 17025 요구사항 준수

**Proficiency Testing Programs**
- 정기적 외부 품질 평가 참여
- 측정 능력 객관적 검증
- 국제 표준과의 추적성 확인
- 지속적 개선 계획 수립

## Reproducibility Assurance Framework

### CERN Analysis Preservation System
**Container Technology Integration**
- Docker 컨테이너를 통한 완전한 환경 보존
- Kubernetes 오케스트레이션으로 확장성 확보
- CernVM-FS와의 통합으로 대용량 데이터 처리
- "Lazy containers"로 효율적 리소스 활용

**REANA Platform Implementation**
```yaml
reana_workflow:
  inputs:
    - raw_data.root
    - analysis_config.yaml
  workflow:
    type: yadage
    specification: analysis_workflow.yaml
  outputs:
    - results_plots/
    - statistical_analysis.json
```

### Blind Analysis Protocols
**Class A Blinding (신호 영역 차단)**
- 분석 절차 확정까지 신호 영역 접근 금지
- 사이드밴드를 이용한 배경 추정
- 절차 확정 후 일괄 언블라인딩
- 편향 제거와 객관성 확보

**Class B Blinding (데이터 시프트)**
- 통계적 특성 유지하며 데이터 변환
- 알려지지 않은 오프셋 적용
- 상대적 변화량은 보존
- 분석 완료 후 오프셋 제거

## Data Integrity & Documentation

### Electronic Lab Notebook (ELN) Systems
**eLabFTW Implementation**
- FAIR 원칙 완전 준수
- 영구 감사 추적 (Audit Trail) 
- 디지털 서명과 타임스탬프
- 실험실 기기와의 자동 통합

**Metadata Schema Design**
```json
{
  "experiment_metadata": {
    "id": "EXP_2024_001",
    "timestamp": "2024-08-20T15:30:00Z",
    "operator": "tsugumi_craftsman",
    "equipment": {
      "instrument_id": "SPEC_001",
      "calibration_date": "2024-08-15",
      "uncertainty": "±0.001%"
    },
    "environmental_conditions": {
      "temperature": "20.0±0.1°C",
      "humidity": "45±5%",
      "pressure": "1013.25±0.1 hPa"
    }
  }
}
```

### Version Control & Code Management
**Git-based Scientific Workflow**
- 실험 절차의 버전 관리
- 코드 리뷰와 품질 보증
- 지속적 통합 (CI) 파이프라인
- 자동 테스트와 검증

**Data Management Plans (DMP)**
- NSF 요구사항에 따른 2페이지 DMP
- 데이터 타입과 메타데이터 명세
- 접근성과 보존 계획
- 재사용과 재배포 정책

## Specialized Instrumentation Techniques

### Ultra-High Vacuum (UHV) Systems
**Pressure Achievement Protocols**
- 10⁻⁹ Torr 미만 달성을 위한 다단계 펌핑
- 터보분자 펌프 + 이온 펌프 조합
- 180°C에서 베이킹을 통한 탈가스
- 잔류 가스 분석기를 통한 누출 검출

**Materials & Contamination Control**
- UHV 호환 재료만 사용 (플라스틱, PTFE 금지)
- 스테인리스 스틸 316LN과 무산소 구리
- 클린룸 절차와 입자 제어
- 분자층 오염 방지 프로토콜

### Cryogenic & High-Field Systems
**Dilution Refrigerator Operation**
- ³He-⁴He 혼합물을 이용한 1mK 달성
- 다중 온도 스테이지 관리
- 열 차단과 진동 격리
- 온도 측정의 정확성과 안정성

**Superconducting Magnet Management**
- 7T 이상 자기장에서 온도 제어
- 퀀치 보호와 헬륨 회수 시스템
- 자기장 균일성과 안정성 확보
- 잔류 자기장 측정과 보정

## Advanced Error Analysis

### Systematic Uncertainty Assessment
**Component-by-Component Analysis**
- 각 불확실성 소스의 독립적 평가
- 상관관계 매트릭스 구성
- 민감도 분석을 통한 주요 기여자 식별
- 개선 우선순위 결정

**Cross-Check Methods**
- 독립적 측정 방법과의 비교
- 이론적 예측값과의 일치성 검증
- 다른 실험실 결과와의 상호 검증
- 메타 분석을 통한 체계적 편향 탐지

### Uncertainty Budget Development
```python
class UncertaintyBudget:
    def __init__(self):
        self.components = {}
        self.correlations = {}
    
    def add_component(self, name, value, uncertainty_type, distribution='normal'):
        self.components[name] = {
            'value': value,
            'uncertainty': uncertainty,
            'type': uncertainty_type,  # 'A' or 'B'
            'distribution': distribution
        }
    
    def calculate_combined(self):
        """GUM 방법과 Monte Carlo 방법 모두 지원"""
        return combined_uncertainty, expanded_uncertainty
```

## Field-Specific Implementations

### Particle Physics Precision
- 검출기 교정: 뮤온을 표준으로 한 셀별 교정
- 방사선 손상 모니터링과 보상
- 트리거 효율성 측정과 최적화
- 배경 추정의 체계적 불확실성

### Condensed Matter Precision  
- STM/AFM: 0.1 Å 수준 위치 제어
- 단일 원자 팁 제작과 검증
- 터널링 스펙트로스코피 정밀도
- 표면 준비와 청정도 확인

### Quantum Physics Precision
- 큐비트 충실도 95% 이상 달성
- 결맞음 시간 (T₁, T₂) 극대화
- 양자 상태 토모그래피 정확성
- 오류 보정 임계값 달성