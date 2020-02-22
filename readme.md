## No preprocessing

v0: 136 x 236로 학습 (0.9706)

v2: 128 x 128로 크기 변환, Pretrained weight를 layer3까지만 사용 (0.9687)

v3: 128 x 128로 크기 변환, Pretrained weight를 layer3까지만 사용, Separate Head로 변경 (0.9669)

v4: v3 + GeM (0.9693)

v5: v2, DataGeneration, alpha = 1 (worse than v2)

v6: v2 + GeM (worse than v2)

v7: v4 + cutout, alpha=0.4, loss 2:1:1, not preprocessed

v8: v4 + MISH, loss = 1:1:1

v9: v7 + original image (epoch 50부터는 aug 2배로)

v10: v7 + erase cutmix (worse than v7)

v11: preprocessed, 128

<!---

## No Preprocessing



#> 경로: military_yolact/yolact_plate/yolact_pngFile_plate.py

#> 기능 및 변경사항: 식판, 손, 숫가락, 젓가락만을 분할(segmentation)합니다.

#> 사용법: calcVolume_m_yolact.py를 위해 평소에는 comment 처리합니다.

#* Input : trained_model_path, path

#* Output: 식판, 손, 숫가락, 젓가락 모델의 예측 결과가 사진으로 나타납니다.

-->
