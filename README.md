# -Mini-project-image-processing-
โปรเจคนี้เป็นการสร้าง ภาพหมอก (Haze) จากภาพถ่ายปกติ โดยใช้เทคนิค Monocular Depth Estimation 
จาก Model ที่ถูกเทรนมาก่อนของ Monodepth2 [https://github.com/nianticlabs/monodepth2](https://github.com/nianticlabs/monodepth2.git) เเละ 
ใช้ Haze Synthesis ของ tranleanh [https://github.com/tranleanh/haze-synthesis.git](https://github.com/tranleanh/haze-synthesis.git) เป็นโครงสร้างหลัก 
ซึ่งใช้โครงสร้างพื้นฐานของ PyTorch และ OpenCV ในการประมวลผล
# วัตถุประสงค์ของโปรเจค
1.สร้างภาพหมอกจากภาพปกติ
2.ปรับระดับความหนาของหมอกได้ตามค่า Beta 1(หมอกบาง), 1.5(หมอกปานกลาง), 2(หมอกหนา)
3.ใช้ Model Monodepth2 เพื่อสร้างเอฟเฟกต์หมอกในภาพ

