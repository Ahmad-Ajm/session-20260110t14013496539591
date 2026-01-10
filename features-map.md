# Features Map – Project Feature Inventory

هذا الملف هو الخريطة المركزية لجميع الميزات (Features / Epics) في المشروع.
التطبيق: واجهة رسومية مكتبية لـ ffmpeg (Python / Windows)

---

## 1. نظرة عامة – جدول الميزات

| FeatureId      | FeatureName                         | FeatureType    | Summary                                                     | Personas        | Requirements              | SpecFolders                     | Priority | Status   |
|----------------|-------------------------------------|----------------|-------------------------------------------------------------|-----------------|---------------------------|----------------------------------|----------|----------|
| FEAT-GUI-CORE  | واجهة التطبيق الأساسية               | CRUD           | واجهة رسومية عربية لإدارة وتشغيل عمليات ffmpeg              | User            | FR-01, NFR-01             | ui, core                        | P0       | Planned  |
| FEAT-FILE-MGR  | إدارة الملفات                        | CRUD           | اختيار الملفات، السحب والإفلات، وتحديد مسار الحفظ            | User            | FR-02, NFR-02             | ui, filesystem                  | P0       | Planned  |
| FEAT-FFMPEG-OPS| عمليات ffmpeg الجاهزة                | Workflow       | تنفيذ عمليات شائعة (تحويل، تقطيع، جودة) عبر واجهة مبسطة     | User            | FR-03                    | ffmpeg, workflows               | P0       | Planned  |
| FEAT-CMD-CUST  | تخصيص أوامر ffmpeg                   | Workflow       | إدخال أوامر ffmpeg مخصصة وتشغيلها                            | User            | FR-04                    | ffmpeg, workflows               | P1       | Planned  |
| FEAT-HISTORY   | سجل العمليات                         | Reporting      | عرض سجل العمليات السابقة وإعادة تنفيذها                     | User            | FR-05                    | history, storage                | P1       | Planned  |
| FEAT-NOTIFY    | الإشعارات والتنبيهات                 | Notifications  | إشعارات نجاح/فشل التنفيذ وحالة التقدم                        | User            | FR-06                    | notifications                   | P1       | Planned  |
| FEAT-FFMPEG-SET| إعداد ffmpeg                         | Integration    | التحقق من ffmpeg أو تحميله وتهيئته                           | User            | NFR-03                   | integration, ffmpeg             | P0       | Planned  |

---

## 2. تفاصيل الميزات

### FEAT-GUI-CORE – واجهة التطبيق الأساسية
**Type:** CRUD  
**Summary:** واجهة رسومية عربية بسيطة لإدارة وتشغيل جميع وظائف التطبيق.  
**Personas:** User  
**Requirements:** FR-01, NFR-01  
**Spec Folders / Files:**  
- `specifications/ui/`  
- `specifications/core/`

**Dependencies / Relations:**  
- تعتمد على: FEAT-FILE-MGR, FEAT-FFMPEG-OPS  
- تؤثر على: جميع الميزات الأخرى

**KPI Template:**  
- `specifications/12-testing/kpi-crud-template.md`

**Recommended Feature Prompt (Cursor):**  
- `cursor_prompt_feature-crud.txt`

**Notes / Open Questions:**  
- اختيار إطار GUI (Tkinter / PySide / PyQt).

---

### FEAT-FILE-MGR – إدارة الملفات
**Type:** CRUD  
**Summary:** تمكين المستخدم من اختيار الملفات والسحب والإفلات وتحديد مسار الحفظ.  
**Personas:** User  
**Requirements:** FR-02, NFR-02  
**Spec Folders / Files:**  
- `specifications/filesystem/`

**Dependencies / Relations:**  
- تعتمد على: FEAT-GUI-CORE  
- تؤثر على: FEAT-FFMPEG-OPS

**KPI Template:**  
- `specifications/12-testing/kpi-crud-template.md`

**Recommended Feature Prompt (Cursor):**  
- `cursor_prompt_feature-crud.txt`

---

### FEAT-FFMPEG-OPS – عمليات ffmpeg الجاهزة
**Type:** Workflow  
**Summary:** تنفيذ عمليات ffmpeg الشائعة عبر نماذج جاهزة.  
**Personas:** User  
**Requirements:** FR-03  
**Spec Folders / Files:**  
- `specifications/ffmpeg/workflows.md`

**Dependencies / Relations:**  
- تعتمد على: FEAT-FILE-MGR, FEAT-FFMPEG-SET

**KPI Template:**  
- `specifications/12-testing/kpi-workflow-template.md`

**Recommended Feature Prompt (Cursor):**  
- `cursor_prompt_feature-workflow.txt`

---

### FEAT-CMD-CUST – تخصيص أوامر ffmpeg
**Type:** Workflow  
**Summary:** إدخال أوامر ffmpeg يدويًا وتشغيلها.  
**Personas:** User  
**Requirements:** FR-04  
**Spec Folders / Files:**  
- `specifications/ffmpeg/custom.md`

**Dependencies / Relations:**  
- تعتمد على: FEAT-FFMPEG-SET

**KPI Template:**  
- `specifications/12-testing/kpi-workflow-template.md`

---

### FEAT-HISTORY – سجل العمليات
**Type:** Reporting  
**Summary:** تخزين وعرض سجل العمليات السابقة مع إعادة التنفيذ.  
**Personas:** User  
**Requirements:** FR-05  
**Spec Folders / Files:**  
- `specifications/history/`

**Dependencies / Relations:**  
- تعتمد على: FEAT-FFMPEG-OPS

**KPI Template:**  
- `specifications/12-testing/kpi-reporting-template.md`

---

### FEAT-NOTIFY – الإشعارات والتنبيهات
**Type:** Notifications  
**Summary:** تنبيهات حالة التنفيذ والأخطاء.  
**Personas:** User  
**Requirements:** FR-06  
**Spec Folders / Files:**  
- `specifications/notifications/`

**Dependencies / Relations:**  
- تعتمد على: FEAT-FFMPEG-OPS

**KPI Template:**  
- `specifications/12-testing/kpi-notifications-template.md`

---

### FEAT-FFMPEG-SET – إعداد ffmpeg
**Type:** Integration  
**Summary:** التحقق من وجود ffmpeg أو تحميله وتهيئته.  
**Personas:** User  
**Requirements:** NFR-03  
**Spec Folders / Files:**  
- `specifications/integration/ffmpeg.md`

**Dependencies / Relations:**  
- تؤثر على: جميع ميزات ffmpeg

**KPI Template:**  
- `specifications/12-testing/kpi-integration-template.md`
