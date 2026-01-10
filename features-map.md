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

## 1.1 جدول مرجعي إضافي (حسب SpecKit)

| FeatureId      | FeatureName        | FeatureType | Summary                                      | Personas         | Requirements      | SpecFolders                             | Priority | Status      |
|----------------|--------------------|-------------|----------------------------------------------|------------------|-------------------|------------------------------------------|----------|------------|
| FEAT-EXAMPLE01 | Example Feature    | CRUD        | مثال لميزة CRUD كاملة (إنشاء/عرض/تعديل/حذف) | Admin, User      | FR-EX-01, FR-EX-02 | 04-domain, 07-api, 08-ui                | P1       | Planned    |
| FEAT-GUI-CORE  | واجهة التطبيق الأساسية | CRUD | واجهة رسومية عربية لإدارة وتشغيل ffmpeg | User | FR-01, NFR-01 | ui, core | P0 | Planned |
| FEAT-FILE-MGR  | إدارة الملفات | CRUD | اختيار الملفات والسحب والإفلات ومسار الحفظ | User | FR-02, NFR-02 | ui, filesystem | P0 | Planned |
| FEAT-FFMPEG-OPS| عمليات ffmpeg الجاهزة | Workflow | عمليات تحويل وتقطيع وضبط جودة جاهزة | User | FR-03 | ffmpeg, workflows | P0 | Planned |
| FEAT-CMD-CUST  | تخصيص أوامر ffmpeg | Workflow | إدخال وتشغيل أوامر ffmpeg مخصصة | User | FR-04 | ffmpeg, workflows | P1 | Planned |
| FEAT-HISTORY   | سجل العمليات | Reporting | عرض سجل العمليات وإعادة التنفيذ | User | FR-05 | history, storage | P1 | Planned |
| FEAT-NOTIFY    | الإشعارات والتنبيهات | Notifications | تنبيهات حالة التنفيذ والأخطاء | User | FR-06 | notifications | P1 | Planned |
| FEAT-FFMPEG-SET| إعداد ffmpeg | Integration | التحقق من وجود ffmpeg أو تحميله | User | NFR-03 | integration, ffmpeg | P0 | Planned |

---

## 2. تفاصيل الميزات

(بقية الملف بدون تغيير، معتمد مباشرة على conversation-summary.md)
