# AIB-tantai
# Deepfake Video Classification
ในปัจจุบัน เทคโนโลยี Deepfake ที่สามารถปลอมแปลงใบหน้าในวิดีโอได้อย่างแนบเนียน กำลังเป็นภัยคุกคามที่เพิ่มขึ้นอย่างรวดเร็ว ทั้งการหลอกลวงทางการเงิน การสร้างข่าวปลอม และการปลอมแปลงตัวตน
ผมเห็นข่าวมิจฉาชีพปลอมเป็นเจ้าหน้าที่ตำรวจหรือคนรู้จัก โทรมาหลอกเอาเงินจากผู้สูงอายุอยู่บ่อยครั้ง และเมื่อ Deepfake เข้าถึงได้ง่ายขึ้น คนทั่วไปก็มีโอกาสตกเป็นเหยื่อมากขึ้น
ผมจึงอยากพัฒนา Model AI ที่ช่วยตรวจจับวิดีโอ Deepfake เพื่อให้ทุกคนสามารถตรวจสอบความน่าเชื่อถือของวิดีโอ ก่อนที่จะตัดสินใจเชื่อหรือทำตามที่วิดีโอนั้นบอก

# Dataset
ในส่วนขอ dataset ผมจะมีของส่วนคือ real video กับ deepfake video ในส่วนของ real video ผมหามาจากใน Kaggle ดังนี้

Real VS Fake - Liveness Detection Dataset
Classification of real videos and replay attacks of people - face anti spoofing
www.kaggle.com

Anti-Spoofing Dataset, 30,000 sets
Biometric Attack dataset for the anti-spoofing task
www.kaggle.com

Anti Spoofing Real Dataset - 87,340 files
43,670 sets of files - Biometric Attack dataset
www.kaggle.com

FaceForensics++ Dataset (C23)
This the faceforensics++ dataset with deepfake and original videos.
www.kaggle.com

และในส่วนของ deepfake video ผมใช้วิดีโอของ

FaceForensics++ Dataset (C23)
This the faceforensics++ dataset with deepfake and original videos.
www.kaggle.com

สลับกับใบหน้าของ

Human Faces Dataset
Real and AI-generated Human Face Images (around 5k each)
www.kaggle.com

โดยใช้โมเดล InsightFace ในการสลับใบหน้า

และต่อมาผมจะแบ่งชุดข้อมูลออกเป็น 3 Set ดังนี้

Train Set 70%

Validation Set 10%

Test Set 20%

โดยใช้ตัวของ scikit learn ในการแบ่ง
