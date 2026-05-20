@"
# Dental Görüntülerde Çürük ve Mikro Hasar Tespiti

Bu proje, dental görüntüler üzerinde çürük, derin çürük, periapikal lezyon ve diş yüzeyi hasarı/aşınması gibi patolojik bulguların derin öğrenme tabanlı modellerle tespit edilmesini amaçlamaktadır.

## Kullanılan Veri Setleri

- DENTEX 2023
- AlphaDent
- Intraoral Caries Dataset

## Kullanılan Modeller

- YOLOv8
- YOLOv8-seg
- YOLO11
- YOLO11-seg
- RT-DETR-l
- DeepLabV3+ ResNet34

## Görevler

- Object Detection
- Instance Segmentation
- Semantic Segmentation

## Final Sonuçlar

| Veri Seti | Görev | Final Model | Ana Metrik |
|---|---|---|---|
| DENTEX 2023 | Object Detection | RT-DETR-l | mAP50 = 0.0229 |
| AlphaDent | Instance Segmentation | YOLOv8m-seg | mask mAP50 = 0.6121 |
| Intraoral Caries | Object Detection | RT-DETR-l | mAP50 = 0.9503 |
| AlphaDent / DeepLabV3+ | Semantic Segmentation | DeepLabV3+ ResNet34 | val mIoU = 0.3729 |

## Proje Klasörleri

- `notebooks/`: Veri hazırlama, model eğitimi ve sonuç analiz notebookları
- `results/`: Model karşılaştırma tabloları, metrikler ve genel sonuç dosyaları

## Not

Veri setleri, eğitim çıktıları ve büyük model ağırlıkları dosya boyutu nedeniyle repoya dahil edilmemiştir. Bu dosyalar Google Drive üzerinde tutulmuştur.
"@ | Set-Content README.md -Encoding UTF8

git add README.md
git commit -m "README dosyasi eklendi"
git push
