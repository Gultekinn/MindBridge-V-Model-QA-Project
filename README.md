# 🚀 MindBridge V-Model QA & Kanban Integration Project

<div align="center">

| **Author** | **Date** | **Metodologiya** | **İdarəetmə Aləti** |
| :---: | :---: | :---: | :---: |
| **Əzizova Gültəkin** | 26.09.2026 | V-Model (Verification & Validation) | Jira/Kanban |

</div>

---

## 📌 Project Overview
Bu layihə Coursera MindBridge QA kursu çərçivəsində **V-Model** mərhələlərinin **Jira Kanban** lövhəsində əlaqələndirilməsi üzrə praktik işdir. Mövcud CSV və ekran görüntüləri 9 ticket-in sütunlar üzrə təşkilini göstərir; layihə ayrıca test icralarının və ya real işəgötürən layihəsinin sübutu kimi təqdim edilmir.

**Tarix qeydi:** CSV-dəki yaradılma tarixləri və ekran görüntüləri 26 sentyabr 2026-nı göstərir. Orijinal PDF-də yazılmış `26.09.2016` bu materiallarla uyğun gəlmir; PDF dəyişdirilmədən saxlanılıb, README-də sübuta uyğun 2026 istifadə olunub. Portfolio review: **5 noyabr 2026**.

---

## 🏗️ V-Model & Kanban Arxitekturası
Jira lövhəsində test növləri V-Model məntiğinə uyğun olaraq mərhələli şəkildə paylanmışdır:
- **Verification (Yoxlama):** Sol sütunlar (*Requirements and Test Planning*, *System Design and Test Design*).
- **Validation (Təsdiqləmə/İcra):** Sağ sütunlar (*System and Integration Testing*, *Acceptance Testing*, *Done*).

Sütunlar kursun sadələşdirilmiş workflow-udur. Unit testlərin hazırlanması verification ilə, onların icrası isə validation ilə əlaqəlidir; `Done` ayrıca V-Model test səviyyəsi deyil, iş statusudur. Ticket-in sütunda yerləşməsi həmin testin həqiqətən icra edildiyini göstərmir.

### 🧩 9 ticket-in izlənməsi

| Sütun | Ticket-lər | Say |
| --- | --- | --- |
| Requirements and Test Planning | KAN-10 — Draft Acceptance Test Plan | 1 |
| System Design and Test Design | KAN-11 — Draft System Test Plan; KAN-12 — Write Integration Test Cases | 2 |
| Development and Unit Testing | KAN-13 — Define Unit Test Cases; KAN-14 — Execute Unit Tests | 2 |
| System and Integration Testing | KAN-7 — Execute Integration Test Suite; KAN-8 — Perform Security Scan | 2 |
| Acceptance Testing and Sign-off | KAN-15 — Run UAT Scenarios | 1 |
| Done | KAN-16 — Conduct Exploratory Testing | 1 |

**Cəmi: 1 + 2 + 2 + 2 + 1 + 1 = 9.** CSV-də KAN-9 yoxdur; KAN-7-dən KAN-16-ya qədər bütün ardıcıl nömrələrin mövcud olduğunu güman etmək olmaz. PDF unit test dizaynını və icrasını bir sətirdə birləşdirir, CSV və board isə onları iki ayrıca ticket kimi göstərir.

### 📊 1. Jira Kanban Lövhəsi (Board View)
Layihənin iş axını və tapşırıqların sütunlar üzrə paylanması:

![Kanban Board](./Screenshot%202026-09-26%20182007.png)
### 📋 2. Issues List View
CSV-dəki 9 ticket-in statusları və detalları (KAN-7, KAN-8 və KAN-10–KAN-16):

![Issues List](./Screenshot%202026-09-26%20181953.png)
---

## 📁 Layihə Faylları və Resursları


- 📄 **Ətraflı Laboratoriya Hesabatı (PDF):** [MindBridge V-Model QA Lab Report.pdf](./MindBridge%20V-Model%20QA%20Lab%20Report.pdf)
- 📊 **Jira İxrac Faylı (CSV):** [Jira.csv](./Jira.csv)

## 🔎 Sübutların əhatəsi

- CSV və board görüntüsündəki 9 ticket bir-biri ilə tutuşdurulub.
- CSV-də yalnız KAN-16 `Tamam` statusundadır; qalanları digər workflow statuslarındadır. Bu, bütün test işlərinin tamamlanması və ya production sign-off demək deyil.
- Test planlarının məzmunu, unit/integration test kodu, security scan output-u, UAT nəticələri və ayrıca retest log-u təqdim olunmayıb. Ticket adlarını faktiki icra nəticəsi kimi saymaq olmaz.
- Orijinal PDF, CSV və ekran görüntüləri dəyişdirilməyib; bu yeniləmə README-də tarix, say və sübut sərhədlərini dəqiqləşdirir.

---

