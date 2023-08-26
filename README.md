# Seq2Seq 영어-프랑스어 번역기

텐서플로를 활용하여 `Seq2Seq` 모델로 영어와 프랑스어 간의 번역기를 구현해보았습니다. 이번 구현에서는 **배치 학습 (Batch Training)** 을 중점적으로 적용하였습니다.

## 📝 프로젝트 개요

- 텐서플로의 구조가 "define and run" 방식이므로 중간마다 **check point**를 설정하여 학습의 안정성을 확보하였습니다.
- 기본 제공되는 `seq2seq` 툴 대신 **dynamic**한 접근법으로 직접 모델을 설계하고 구현하였습니다.
- 전체 파일 구조는 총 4개의 ipython 파일로 되어 있으며, `main` 실행 시 나머지 세 파일이 자동으로 임포트됩니다.

## 💡 주요 특징

- **Batch Training**: 효율적인 학습을 위해 배치 학습 기법을 적용하여 데이터를 일괄 처리하였습니다.
- **Encoder와 Decoder 분리**: Encoder와 Decoder를 별도의 구조로 설계하여 더욱 세밀한 조절과 최적화를 가능하게 하였습니다.
- **Dynamic Seq2Seq**: 미리 정의된 텐서플로 그래프를 유연하게 수정하고 활용하였습니다.
- **Attention Mechanism**: Decoder 내에서 dot product 방식의 attention을 통해 번역의 정확도를 높였습니다.

## 📚 공부 내용

텐서플로를 활용하여 다음과 같은 핵심 내용들에 대해 깊이 있게 연구하고 학습하였습니다:

- `get_variable_scope`, `get_variable`, `variable_scope`
- `tf.scan`의 다양한 활용법
- `place_holder`, `sparse_place_holder` 등의 사용법

## 📌 참고

이 프로젝트는 pytorch tutorial을 참조하여 작성되었습니다. 따라서, 일부 유사한 구조나 내용이 포함되어 있을 수 있습니다.

