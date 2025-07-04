# Examples - ตัวอย่างการใช้งาน

โฟลเดอร์นี้มีตัวอย่างการใช้งาน RAG-Chain Chatbot แบบต่างๆ เหมาะสำหรับการเรียนรู้และทดสอบระบบ

## 📋 รายการตัวอย่าง

### 🤖 Basic Usage Examples
- **[basic_rag_example.py](basic_rag_example.py)** - การใช้งาน RAG พื้นฐาน
- **[simple_chatbot.py](simple_chatbot.py)** - แชทบอทขายของแบบง่าย

### 📚 Data Management Examples  
- **[data_ingestion_example.py](data_ingestion_example.py)** - การ ingest และประมวลผลข้อมูล

### 📝 Prompt Management Examples
- **[prompt_templates_example.py](prompt_templates_example.py)** - การใช้งาน prompt templates

## 🚀 วิธีการรัน

### ข้อกำหนดเบื้องต้น
```bash
# ติดตั้ง dependencies
uv sync

# ตั้งค่า API key
cp config.example.yaml config.yaml
# แก้ไข config.yaml ใส่ OpenAI API key ของคุณ
```

### รันตัวอย่าง
```bash
# ตัวอย่างพื้นฐาน
python examples/basic_rag_example.py

# แชทบอทง่าย
python examples/simple_chatbot.py

# การ ingest ข้อมูล
python examples/data_ingestion_example.py

# การใช้งาน prompt templates
python examples/prompt_templates_example.py
```

## 📖 คำอธิบายตัวอย่าง

### 🤖 basic_rag_example.py
**สำหรับ**: ผู้เริ่มต้นที่ต้องการเข้าใจการทำงานพื้นฐาน
- โหลดการตั้งค่าและระบบ RAG
- ทดสอบคำถามตัวอย่าง
- โหมดสนทนาแบบง่าย

### 💬 simple_chatbot.py  
**สำหรับ**: การสร้างแชทบอทขายของที่มี UX ดี
- ระบบทักทายและแนะนำ
- คำแนะนำคำถามด่วน
- การติดตามประวัติการสนทนา
- คำสั่งพิเศษ (help, summary)

### 📚 data_ingestion_example.py
**สำหรับ**: การเรียนรู้กระบวนการประมวลผลข้อมูล
- ตรวจสอบไฟล์ข้อมูล
- การแบ่งเอกสาร (chunking)
- การสร้าง FAISS index
- การทดสอบการค้นหา

### 📝 prompt_templates_example.py
**สำหรับ**: การจัดการและใช้งาน prompt templates
- การโหลดและใช้งาน templates
- การ format templates พร้อมตัวแปร
- การสร้าง template ใหม่

## 💡 Tips การใช้งาน

### เริ่มต้นใหม่?
1. เริ่มจาก `basic_rag_example.py`
2. ลองใช้ `simple_chatbot.py` 
3. เรียนรู้ data management จาก `data_ingestion_example.py`

### ต้องการปรับแต่ง?
1. ดู `prompt_templates_example.py` สำหรับการจัดการ prompts
2. ใช้ `data_ingestion_example.py` สำหรับการเรียนรู้การจัดการข้อมูล

## 🔧 การแก้ปัญหา

**ไม่พบไฟล์ข้อมูล**
- ตรวจสอบว่ามีไฟล์ในโฟลเดอร์ `data/raw/`
- ตัวอย่างจะสร้างไฟล์ตัวอย่างให้หากไม่พบ

**API Key Error**  
- ตรวจสอบไฟล์ `config.yaml`
- ตรวจสอบ credits ใน OpenAI dashboard

**Import Error**
- รัน `uv sync` เพื่อติดตั้ง dependencies
- ตรวจสอบว่าอยู่ในโฟลเดอร์โปรเจกต์

## 🔗 เอกสารเพิ่มเติม

- [Quick Start Guide](../docs/quickstart.md) - เริ่มต้นใช้งาน
- [Complete Documentation](../docs/README.md) - เอกสารทั้งหมด 