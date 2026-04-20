# 🤖 Smart WhatsApp Multi-Agent Assistant

> An advanced, fully automated WhatsApp AI Assistant built on a Multi-Agent Architecture. This project serves as a dynamic Orchestrator that intelligentally routes user requests to specialized AI sub-agents to execute complex daily tasks seamlessly.

## 📌 Project Overview
This repository showcases the architecture and capabilities of a custom-built AI Assistant. Instead of relying on a single, easily overloaded AI model, this system utilizes a **Supervisor/Worker (Orchestrator & Child Agents)** design pattern. It processes text, voice, and image inputs via WhatsApp and performs real-world actions like scheduling, emailing, and web searching.

*Note: The source code and environment variables are kept private for security purposes. This repository serves as a technical showcase.*

<img width="1505" height="810" alt="image" src="https://github.com/user-attachments/assets/2b1e3a6e-78ce-47ea-8db6-ba61073b4071" />

## ⚙️ Architecture & Workflow
1. **Input Layer:** Receives text, audio, or images via WhatsApp Cloud API.
2. **The Orchestrator Agent:** Powered by the highly capable `Gemini 3.1 Pro`. It analyzes the user's intent, extracts context, and delegates the task to the appropriate specialized agent.
3. **Specialized Child Agents:** Powered by the ultra-fast `Gemini 3.1 Flash` to ensure rapid response times and cost efficiency:
   - 📅 **Calendar Agent:** Manages Google Calendar (Create, Update, Delete events) with strict timezone handling.
   - 📧 **Email Agent:** Drafts and sends professional emails via Gmail API.
   - 🔍 **Web Search Agent:** Fetches real-time data using Google Search, Wikipedia, and Hacker News.
   - 🐦 **Social Media Agent:** Generates and drafts social media posts (e.g., X/Twitter).
   - 📂 **RAG Agent:** Retrieves information from custom PDF documents using Pinecone Vector DB.
4. **Output Layer:** Returns the final formatted response (text or synthesized voice) back to the user on WhatsApp.

## 🛠️ Tech Stack
* **Workflow Automation:** n8n (Self-hosted)
* **AI Models:** Google Gemini 3.1 Pro (Orchestrator) & Gemini 3.1 Flash (Workers)
* **Vector Database:** Pinecone
* **Integrations:** WhatsApp Cloud API, Google Calendar API, Gmail API, Google Custom Search.

## 👨‍💻 Developed By
**Adel Mohamed Mohamed Diab**
*Information Technology (IT) Student & Systems Automation Enthusiast.*
---
# 🤖 المساعد الذكي متعدد الوكلاء عبر واتساب (Multi-Agent System)

> مساعد ذكي متطور ومؤتمت بالكامل يعمل عبر تطبيق واتساب، مبني على معمارية "الوكلاء المتعددين" (Multi-Agent Architecture). يعمل هذا النظام كمدير ذكي (Orchestrator) يقوم بتوجيه طلبات المستخدم إلى وكلاء ذكاء اصطناعي متخصصين لتنفيذ المهام المعقدة بسلاسة.

## 📌 نظرة عامة على المشروع
يعرض هذا المستودع الهيكلية والقدرات التقنية لمساعد ذكي تم تطويره برمجياً. بدلاً من الاعتماد على نموذج ذكاء اصطناعي واحد يسهل إرهاقه، يستخدم هذا النظام نمط (المدير والموظفين). حيث يعالج المدخلات النصية والصوتية والصور عبر واتساب، وينفذ مهام حقيقية مثل جدولة المواعيد، إرسال الإيميلات، والبحث على الإنترنت.

*ملاحظة: الكود المصدري ومتغيرات البيئة (البيانات السرية) محفوظة بشكل خاص لدواعي الأمان. هذا المستودع بمثابة عرض تقني للمشروع.*

<img width="1505" height="810" alt="image" src="https://github.com/user-attachments/assets/174b48b6-67a2-48e7-ae59-d4500123df16" />

## ⚙️ معمارية النظام وآلية العمل
1. **طبقة الاستقبال (Input):** استقبال الرسائل (نص، صوت، صور) عبر واجهة (WhatsApp Cloud API).
2. **الوكيل المدير (Orchestrator):** يعمل بنموذج `Gemini 3.1 Pro` فائق الذكاء. وظيفته تحليل نية المستخدم، وفهم السياق، وتفويض المهمة للوكيل المتخصص المناسب.
3. **الوكلاء المتخصصون (Child Agents):** تعمل بنموذج `Gemini 3.1 Flash` فائق السرعة لضمان استجابة لحظية وتوفير في الموارد:
   - 📅 **وكيل التقويم:** إدارة مواعيد Google Calendar (إنشاء، تعديل، حذف) مع معالجة دقيقة لفروق التوقيت.
   - 📧 **وكيل البريد الإلكتروني:** صياغة وإرسال رسائل بريد إلكتروني احترافية عبر Gmail API.
   - 🔍 **وكيل البحث:** جلب بيانات لحظية باستخدام بحث جوجل، ويكيبيديا، وHacker News.
   - 🐦 **وكيل السوشيال ميديا:** صياغة وتجهيز منشورات لوسائل التواصل الاجتماعي (مثل منصة X).
   - 📂 **وكيل المستندات (RAG):** استخراج المعلومات من ملفات الـ PDF الخاصة باستخدام قاعدة بيانات Pinecone.
4. **طبقة الإرسال (Output):** إرسال النتيجة النهائية المنسقة (كنص أو صوت بشري) للمستخدم عبر واتساب.

## 🛠️ التقنيات المستخدمة
* **أتمتة سير العمل:** n8n
* **نماذج الذكاء الاصطناعي:** Google Gemini 3.1 Pro (للمدير) & Gemini 3.1 Flash (للموظفين)
* **قاعدة البيانات المتجهة:** Pinecone
* **الربط البرمجي (APIs):** واتساب، تقويم جوجل، جيميل، وبحث جوجل.

## 👨‍💻 تطوير
**عادل محمد محمد دياب**
*طالب تكنولوجيا المعلومات (IT) ومُهتم بأتمتة الأنظمة والذكاء الاصطناعي.*
