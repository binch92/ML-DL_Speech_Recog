# Speech_Recog
🔮 감정 음성 데이터 분석: 과적합 방지 고찰


프로젝트 관련 링크
발표용 슬라이드: https://docs.google.com/presentation/d/1ysadmKWzAK9TvJ8QxTdkTegd7T5-nAVor1_x6cmYPDI/edit#slide=id.p

✨ 프로젝트 소개
image

음성데이터에서 특징을 추출하여 기쁨, 당황, 분노, 불안, 슬픔 총 5개의 감정을 분류하는 모델을 설계

mfcc와 mel spectrogram을 이용하여 음성데이터에서 특징을 추출
image

LSTM 모델 사용
image

-> 과적합 발생 !

음성데이터를 8등분 후 랜덤으로 병합
image

랜덤으로 이어붙인 음성데이터에서 mfcc와 mel spectrogram을 이용하여 특징 추출

LSTM, ResNet, Efficient Net, Random Forest 모델을 사용

모델명	train accuracy	test accuracy	top-2 accuracy
LSTM	0.6087	0.4073	0.7120
ResNet	0.6213	0.4653	0.6967
EfficientNet	0.5170	0.4487	0.6947
RandomForset	--	0.4107	--
📜 기술 스택
image

image
