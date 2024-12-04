# Real-Time Speech-to-Text (STT) Learning Roadmap

#### 실시간 시간 STT를 구현하기 위해 필요한 여러 선행 연구와 개념들을 경험 기반으로 학습 로드맵을 작성해봤습니다.<br/>시간 나는대로 틈틈히 작성하면서 로드맵 우측에 블로그 링크를 추가할 예정입니다.
#### Learning Roadmap Link : https://mz-moonzoo.tistory.com/79
-----
### 1. 컨볼루션 신경망 (CNN)
- CNN의 기본 구조와 원리 : https://mz-moonzoo.tistory.com/63
- 필터와 풀링 개념 : https://mz-moonzoo.tistory.com/63
- 음성 데이터 특징 추출 (1D Convolution,2D Convolution) : https://mz-moonzoo.tistory.com/64

### 2. 시퀀스 모델링
- RNN (Recurrent Neural Network)
- LSTM (Long Short-Term Memory)
- GRU (Gated Recurrent Unit)

### 3. 어텐션 메커니즘
- 기본 어텐션의 개념과 작동 원리
- 셀프 어텐션

### 4. 트랜스포머 아키텍처
- Attention is All you need 논문 리뷰 및 구현
- 인코더-디코더 구조
- 멀티헤드 어텐션
- 포지셔널 인코딩

### 5. 음성 신호 처리
- 음성 신호 처리 기본
- 스펙트로그램과 멜 스펙트로그램
- μ-law decompression / μ-law compression
- Bit Conversion, Resampling
- VAD (Voice activity detection)

### 6. 실시간 음성 인식 시스템
- VoIP Infra (VoIP, SIP, PBX...)
- 음성 데이터 스트리밍을 위한 통신 프로토콜 (Socket, TCP/UDP)
- 실시간 음성 신호 수집 및 처리 (Payload, header...)
 
### 7. OpenAI / Whisper
- Whisper 논문 리뷰
- Whisper 모델의 구조 ( CNN + Transformers )
- Whisper Feature Extractor
- Whisper 장점과 한계점
- Whisper 파인튜닝을 위한 데이터 전처리 및 학습 방법

### 8. Faster-Whisper. (Whisper with Ctranslate2)
- Ctranslate2 (파인튜닝한 Whisper를 Ctranslate2를 이용해 Faster-whisper로 변환)
- Faster-Whisper Input data format (주파수, bit)
- Faster-Whisper  Feature Extractor (적절 패킷 단위)
- Faster-Whisper inference Parameters (VAD, word_timestamp...) 
- Faster-Whisper turbo (only 4 decoder layers)

### 9. Whisper-Streming
- Local Agreement
- Prompt tokens
- wordtimestamp

-----
