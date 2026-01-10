# Features Map – Project Feature Inventory

هذا الملف هو الخريطة المركزية لجميع الميزات (Features / Epics) في المشروع.

---

## 2. نظرة عامة – جدول الميزات

| FeatureId | FeatureName | FeatureType | Summary | Personas | Requirements | SpecFolders | Priority | Status |
|----------------|--------------------|-------------|----------------------------------------------|------------------|-------------------|------------------------------------------|----------|------------|
| FEAT-EXAMPLE01 | Example Feature | CRUD | مثال لميزة CRUD كاملة (إنشاء/عرض/تعديل/حذف) | Admin, User | FR-EX-01, FR-EX-02 | 04-domain, 07-api, 08-ui | P1 | Planned |
| FEAT-FILE-BROWSER | File Browser | CRUD | استعراض ملفات الصوت والفيديو مع السحب والإفلات | User | FR-01 | ui/file-browser | P0 | Active |
| FEAT-FFMPEG-EXEC | FFmpeg Execution | Workflow | تنفيذ أوامر ffmpeg ومتابعة التقدم والأخطاء | User | FR-02 | core/ffmpeg | P0 | Active |
| FEAT-PRESETS | Preset Operations | CRUD | عمليات جاهزة (تحويل، تقطيع، جودة) | User | FR-03 | core/presets | P1 | Planned |
| FEAT-HISTORY | Operations History | Reporting | سجل العمليات السابقة وإعادة تنفيذها | User | FR-04 | core/history | P1 | Planned |
| FEAT-NOTIFY | Execution Notifications | Notifications | تنبيهات نجاح/فشل العمليات | User | FR-05 | core/notifications | P1 | Planned |

---

## 3. تفاصيل الميزات

### FEAT-FILE-BROWSER – File Browser
**Type:** CRUD  
**Summary:** تمكين المستخدم من اختيار ملفات الصوت والفيديو عبر الاستعراض أو السحب والإفلات.  
**Personas:** User  
**Requirements:** FR-01  
**Spec Folders / Files:**  
- `ui/file-browser`

**Dependencies / Relations:**  
- تؤثر على: FEAT-FFMPEG-EXEC

---

### FEAT-FFMPEG-EXEC – FFmpeg Execution
**Type:** Workflow  
**Summary:** تشغيل أوامر ffmpeg ومتابعة التقدم والأخطاء.  
**Personas:** User  
**Requirements:** FR-02  
**Spec Folders / Files:**  
- `core/ffmpeg`

**Dependencies / Relations:**  
- يعتمد على: FEAT-FILE-BROWSER

----

## ✅ جدول الميزات المضافة (تنفيذ فعلي)

| FeatureId      | FeatureName              | FeatureType    | Summary                                      | Personas | Requirements | SpecFolders           | Priority | Status  |
|----------------|--------------------------|----------------|----------------------------------------------|----------|--------------|-----------------------|----------|---------|
| FEAT-FILE-BROWSER | File Browser          | CRUD           | استعراض الملفات مع دعم السحب والإفلات        | User     | FR-01        | ui/file-browser       | P0       | Active  |
| FEAT-FFMPEG-EXEC | FFmpeg Execution      | Workflow       | تنفيذ أوامر ffmpeg ومتابعة حالتها            | User     | FR-02        | core/ffmpeg           | P0       | Active  |
| FEAT-PRESETS     | Preset Operations     | CRUD           | عمليات جاهزة للتحويل والتقطيع والجودة         | User     | FR-03        | core/presets          | P1       | Planned |
| FEAT-HISTORY     | Operations History    | Reporting      | حفظ سجل العمليات وإعادة تنفيذها               | User     | FR-04        | core/history          | P1       | Planned |
| FEAT-NOTIFY      | Execution Notifications | Notifications | إشعارات النجاح والفشل أثناء التنفيذ           | User     | FR-05        | core/notifications    | P1       | Planned |

---

## ➕ جدول الميزات (مطلوب الإضافة)

| FeatureId      | FeatureName        | FeatureType | Summary                                      | Personas         | Requirements      | SpecFolders                             | Priority | Status      |
|----------------|--------------------|-------------|----------------------------------------------|------------------|-------------------|------------------------------------------|----------|------------|
| FEAT-EXAMPLE01 | Example Feature    | CRUD        | مثال لميزة CRUD كاملة (إنشاء/عرض/تعديل/حذف) | Admin, User      | FR-EX-01, FR-EX-02 | 04-domain, 07-api, 08-ui                | P1       | Planned    |
| FEAT-FILE-BROWSER | File Browser | CRUD | استعراض ملفات الصوت والفيديو مع السحب والإفلات | User | FR-01 | ui/file-browser | P0 | Active |
| FEAT-FFMPEG-EXEC | FFmpeg Execution | Workflow | تنفيذ أوامر ffmpeg ومتابعة التقدم والأخطاء | User | FR-02 | core/ffmpeg | P0 | Active |
| FEAT-PRESETS | Preset Operations | CRUD | عمليات جاهزة (تحويل، تقطيع، جودة) | User | FR-03 | core/presets | P1 | Planned |
| FEAT-HISTORY | Operations History | Reporting | سجل العمليات السابقة وإعادة تنفيذها | User | FR-04 | core/history | P1 | Planned |
| FEAT-NOTIFY | Execution Notifications | Notifications | تنبيهات نجاح/فشل العمليات | User | FR-05 | core/notifications | P1 | Planned |