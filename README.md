# Mini-Project: Haze Synthesis with Monodepth2
โปรเจคนี้เป็นการสร้างภาพหมอก (Haze) จากภาพถ่ายปกติ โดยใช้เทคนิค **Monocular Depth Estimation**  
- ใช้ **Model ที่ถูกเทรนมาก่อนของ Monodepth2** → [https://github.com/nianticlabs/monodepth2](https://github.com/nianticlabs/monodepth2)  
- ใช้ **Haze Synthesis ของ tranleanh** → [https://github.com/tranleanh/haze-synthesis.git](https://github.com/tranleanh/haze-synthesis.git) เป็นโครงสร้างหลัก  

---

## วัตถุประสงค์ของโปรเจค
1.สร้างภาพหมอกจากภาพถ่ายปกติ  
2.ปรับระดับความหนาของหมอกได้ตามค่า **Beta**:
- **Beta = 1.0** → หมอกบาง  
- **Beta = 1.5** → หมอกปานกลาง  
- **Beta = 2.0** → หมอกหนา  

3.ใช้โมเดล **Monodepth2** เพื่อสร้างเอฟเฟกต์หมอกในภาพ  

---



### Example:
| Beta | ตัวอย่างภาพ | รายละเอียด |
|-------|-------------|------------|
| **ต้นฉบับ** | ![Original](https://raw.githubusercontent.com/Benz3560Fggg88/-Mini-project-image-processing-/main/1/1%20%E0%B9%84%E0%B8%A1%E0%B9%88%E0%B8%A1%E0%B8%B5%E0%B8%AB%E0%B8%A1%E0%B8%AD%E0%B8%81.jpg) | ไม่มีหมอก |
| **Beta = 1.0** | ![Beta 1.0](https://raw.githubusercontent.com/Benz3560Fggg88/-Mini-project-image-processing-/main/1/1_synt1.jpg) | หมอกบาง |
| **Beta = 1.5** | ![Beta 1.5](https://raw.githubusercontent.com/Benz3560Fggg88/-Mini-project-image-processing-/main/1/1_synt1.5.jpg) | หมอกปานกลาง |
| **Beta = 2.0** | ![Beta 2.0](https://raw.githubusercontent.com/Benz3560Fggg88/-Mini-project-image-processing-/main/1/1_synt2.jpg) | หมอกหนา |

