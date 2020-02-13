## No preprocessing

v0: 136 x 236로 학습

v2: 128 x 128로 크기 변환, Pretrained weight를 layer3까지만 사용

v3: 128 x 128로 크기 변환, Pretrained weight를 layer3까지만 사용, Separate Head로 변경

v4: v3+ GeM


<!---

## No Preprocessing



#> 경로: military_yolact/yolact_plate/yolact_pngFile_plate.py

#> 기능 및 변경사항: 식판, 손, 숫가락, 젓가락만을 분할(segmentation)합니다.

#> 사용법: calcVolume_m_yolact.py를 위해 평소에는 comment 처리합니다.

#* Input : trained_model_path, path

#* Output: 식판, 손, 숫가락, 젓가락 모델의 예측 결과가 사진으로 나타납니다.

-->
