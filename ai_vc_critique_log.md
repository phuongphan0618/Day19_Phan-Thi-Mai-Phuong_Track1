
# Pich gốc
1. Pitch memo:
```
1. THE PROBLEM 

   Sinh viên và nghiên cứu sinh phải đọc hàng chục paper cho mỗi topic, mất nhiều ngày chỉ để xác định bài nào đáng đọc sâu. Quá trình literature review lặp lại theo từng deadline, tiêu tốn nhiều thời gian nhưng phần lớn effort lại dành cho việc lọc và skim thay vì hiểu sâu.

2. THE INSIGHT

   - Người dùng không cần AI “đọc thay toàn bộ paper” — họ cần một cách đáng tin để nhanh chóng quyết định paper nào đáng đọc và paper nào có thể bỏ qua. 
   - Vốn không nên thay thế được việc đọc toàn bộ, nhưng thật sự có quá nhiều hướng một chủ đề có thể xoay quanh, và mỗi paper xuất bản ra hàng ngày không phải lúc nào có nội dung đáng chú ý hoặc chất lượng, việc phải đọc khiến cho đối tượng hướng tới - sinh viên và nghiên cứu sinh dễ nản, đặc biệt dưới tình trạng có deadline.


3. THE SOLUTION

   - Sản phẩm cung cấp một hệ thống tìm kiếm và tóm tắt paper theo truy vấn, trả về danh sách các bài liên quan kèm tóm tắt “đủ để ra quyết định”, trích dẫn rõ ràng và metadata để kiểm chứng nhanh.
   - Khác với ChatGPT hoặc các công cụ tóm tắt đơn lẻ, hệ thống tập trung vào **decision support** (rank + summary + synthesis + source-grounded), giúp người dùng chọn đúng paper thay vì chỉ đọc nhanh hơn.
   - AI được sử dụng để tổng hợp thông tin có kiểm soát (grounded summaries and synthesis), trong khi retrieval và ranking kết hợp heuristic để giảm hallucination và tăng độ tin cậy.

4. WHY NOW

   Sự phổ biến của arXiv và các kho học thuật khiến số lượng paper tăng nhanh, vượt quá khả năng xử lý thủ công của người học. Đồng thời, LLM hiện tại đã đủ tốt để tạo summary có nguồn đáng tin, nhưng chưa được đóng gói thành workflow phù hợp với quá trình literature review thực tế.

5. TRACTION / PROOF (số cụ thể)

   - Số người dùng / pilot: 50-80 người dùng thử ban đầu.
   - Aha moment metric: ngưỡng 40-50% user đạt trong session đầu có thể chọn được ít nhất 1-2 paper ưng ý, ~30% quay lại sử dụng trong vòng 7 ngày khi tiếp tục làm assignment / research.
   - LTV/CAC, payback: 2.92x, 4.3 tháng. 

6. THE ASK (1-2 câu)

   Em cần 100,000,000VND–200,000,000VND pre-seed funding để hoàn thiện MVP, tối ưu cost pipeline và đạt ~500–1,000 người dùng hoạt động trong 12 tháng tới. Ngoài ra, cần hỗ trợ từ mentor và các đối tác trong lĩnh vực học thuật để tiếp cận user thật và validate hành vi sử dụng ở quy mô lớn hơn.
```
2. Twitter pitch:
```
MindMesh giúp sinh viên & nghiên cứu sinh quyết định paper nào đáng đọc và sử dụng trong vài phút bằng AI summary và synthesis có nguồn, thay vì mất hàng giờ skimming. Đã có 0–80 users pilot, 45% đạt aha, LTV/CAC 2.92x. Hiện tại đang gọi 100–200M VND để scale lên 1K users.
```

# AI feedback

```Alright—I’m going to treat this like I’ve heard 50 pitches already (because I have), and I’m deciding in under a minute whether you’re another “LLM wrapper” or something worth leaning in on.

---

# **1. THE 8-SECOND TEST**

> *“Sinh viên và nghiên cứu sinh phải đọc hàng chục paper…”*

❌ **This does NOT earn you another 50 seconds.**

Why?

* It’s **generic and overfamiliar**. I’ve heard:

  * “people waste time reading”
  * “too many documents”
  * “information overload”
    → at least 10 times this week.

* It describes **pain**, but not **urgency or cost**.

  * I don’t know:

    * how often this happens
    * what breaks if they don’t solve it
    * why they’d *pay now*

👉 Right now it sounds like:

> “annoying problem”

Not:

> “must-solve problem”

---

### 🔧 Rewrite (stronger hook)

> Graduate students spend days reading papers just to find 2–3 worth citing before a deadline.

Why this works:

* specific output (2–3 papers)
* clear inefficiency
* implicit urgency (deadline)

---

# **2. THE INSIGHT TEST**

## Your claimed insight:

> “Users don’t want AI to read everything—they want help deciding what to read.”

---

## My reaction:

😐 **This is not non-obvious.**

Every AI founder this week says some version of:

* “we’re not replacing, we’re augmenting”
* “we help decision making”

---

## What’s missing?

You’re **describing behavior**, not revealing **a hidden truth**.

---

## The sharper (actually interesting) version:

Here’s what I think your *real* insight is—but you didn’t say it clearly:

> Users don’t trust AI summaries enough to replace reading—but they will trust them to eliminate 70% of papers from consideration.

🔥 That’s stronger because:

* introduces **trust boundary**
* quantifies behavior
* explains *why your product exists*

---

## 🔧 Rewrite (use this):

> Users won’t trust AI to replace reading—but they will trust it to eliminate most papers and narrow what’s worth their time.

Now I’m leaning forward.

---

# **3. THE OPENAI THREAT**

Let me be blunt:

> If OpenAI adds “summarize top papers for a topic with citations” tomorrow…
> **you are dead in your current form.**

---

## Your current “moat”:

* heuristic ranking
* grounded summaries
* workflow

👉 This is not a moat.
This is **implementation detail**.

---

## Where you’re actually weak:

* No proprietary data
* No network effects
* No switching cost
* No distribution advantage

---

## The real question you must answer:

> Why would a user NOT just paste their query into ChatGPT?

---

## If you don’t fix this, you lose.

---

## Potential moat directions (you need ONE):

### 1. **User interaction data (best path)**

* which papers users accept/reject
* build:

  * ranking model
  * personalization

👉 This becomes:

> “we know what *people like you* chose to read”

---

### 2. **Workflow lock-in**

* saved research trails
* citation graph per user
* evolving “literature state”

👉 ChatGPT can’t replicate continuity easily.

---

### 3. **Trust layer**

* verifiable claims tied to exact spans
* auditability

👉 but this is hard—and you’re not there yet.

---

## Right now:

❗ You are **feature-level, not product-level defensible**

---

# **4. THE NUMBERS TEST**

Let’s go line by line.

---

## ❗ “50–80 pilot users”

Fine. Early stage. No issue.

---

## ❗ “45% aha moment”

I don’t buy this without definition.

* What exactly is:

  > “chọn được 1–2 paper ưng ý”

How do you know:

* they actually used it?
* not just clicked?

👉 This is **soft metric**.

---

## ❗ “30% return in 7 days”

This is your **most important number**, and it’s weak.

Why?

* Your own model says:

  > usage is bursty (deadline-based)

So 7-day retention:

* may be noise
* not signal

---

## ❗ “LTV/CAC 2.92x”

🚨 This is the biggest red flag.

You do NOT have enough data to claim this.

At 50–80 users:

* you don’t know:

  * true churn
  * real willingness to pay

👉 This reads as:

> spreadsheet math, not real data

---

## What I’d say in a partner meeting:

> “They’re projecting SaaS metrics onto non-SaaS behavior.”

---

## What you SHOULD say instead:

> Early signals suggest repeat usage during research cycles; monetization and retention are still being validated.

Less sexy. More credible.

---

# **5. THE WEAKEST LINE**

This one:

> “AI được sử dụng để tổng hợp thông tin có kiểm soát…”

---

## Why I’d push hard here:

* It’s **buzzword-heavy**
* “grounded”, “heuristic”, “reduce hallucination”
  → every pitch this week said this

👉 It signals:

> you’re describing HOW, not WHY it matters

---

## 🔧 Rewrite:

> Every summary links back to exact sources so users can verify before trusting the result.

Short. Concrete. User-facing.

---

# 🔚 **Final verdict (what I’d actually think)**

You’re not bad. You’re just:

> ❗ **one level too generic for me to get excited**

---

## What you did well:

* clear user segment
* realistic constraints (not overbuilding MVP)
* awareness of trust problem

---

## What’s missing:

### 💥 1. A sharp, defensible insight

(not “we help decide”)

### 💥 2. A credible moat story

(not “we use heuristics”)

### 💥 3. Honest traction framing

(not pseudo-SaaS metrics)

---

## If you fix just ONE thing:

👉 Make this your core:

> “We don’t replace reading—we eliminate what’s NOT worth reading, reliably.”

Then:

* tie it to behavior
* tie it to data
* tie it to defensibility

```

# Decision: Partial
```
1. THE PROBLEM
Decision: ACCEPT
Lý do:
- Rõ ràng, cụ thể (days, dozens of papers)
- Có context: deadline → tạo urgency
- Đúng với user segment (không generic “knowledge workers”)

2. THE INSIGHT
Decision: PARTIAL
Lý do: 
- Đã chạm đúng trust boundary
- Có differentiation so với “AI replaces everything”
Nhưng: 
- Vẫn hơi “expected” với người đã nghe nhiều AI pitch
- Thiếu một chút specificity / quantification

3. THE SOLUTION
Decision: PARTIAL
Lý do:
- Positioning đúng: decision > speed
- Có so sánh với ChatGPT (good instinct)
Nhưng: 
- Vẫn là feature-level differentiation
- “rank + summary + grounded” = thứ OpenAI có thể build

4. WHY NOW
Decision: ACCEPT
Lý do:
- Correct trend (paper explosion)
- Nhắc đến sự phát triển của LLM

5. TRACTION / PROOF
Decision: PARTIAL
Lý do: 
- Không fake scale quá
- Có activation metric
Nhưng: 
- Aha metric soft, không chứng minh value thật
- 7-day retention misleading khi product chủ yếu "burst usage", không nói lên nheieuf về weekly retention

6. THE ASK
Decision: ACCEPT
Lý do: 
- Rõ số tiền
- Rõ mục tiêu (MVP, cost, users)
- Không overpromise
```

# Pitch final

```
# PITCH MEMO — MindMesh

1. THE PROBLEM

Sinh viên và nghiên cứu sinh phải mất nhiều ngày đọc hàng chục bài báo chỉ để chọn ra một vài bài đáng trích dẫn trước deadline. Phần lớn thời gian bị lãng phí vào việc lọc và skimming, thay vì thực sự hiểu nội dung.

2. THE INSIGHT

Người dùng sẽ không tin AI để thay thế việc đọc — nhưng họ sẽ tin AI để loại bỏ phần lớn các bài không cần thiết và thu hẹp lại những gì thực sự đáng đọc.

3. THE SOLUTION

MindMesh giúp người dùng quyết định nên đọc gì, không chỉ đọc nhanh hơn. Khi nhập một chủ đề, hệ thống trả về danh sách các paper đã được xếp hạng kèm tóm tắt ngắn gọn và liên kết nguồn trực tiếp, giúp người dùng có thể kiểm chứng trước khi tin tưởng.  
Khác với ChatGPT chỉ trả lời từng truy vấn riêng lẻ, MindMesh hỗ trợ workflow nghiên cứu bằng cách kết hợp tìm kiếm, xếp hạng và tóm tắt có nguồn để giảm lượng tài liệu không liên quan cần đọc.

4. WHY NOW

Số lượng bài báo học thuật đang tăng nhanh hơn khả năng xử lý của mỗi cá nhân, đặc biệt trên các nền tảng như arXiv và Semantic Scholar. Đồng thời, các mô hình LLM hiện tại đã đủ tốt để tạo ra các bản tóm tắt có nguồn đáng tin, nhưng chưa được tích hợp vào workflow ra quyết định trong nghiên cứu.

5. TRACTION / PROOF

- 50–80 người dùng thử ban đầu (sinh viên làm thesis / bài tập nghiên cứu)  
- ~45% người dùng trong session đầu xác định được ít nhất 1–2 bài đáng đọc sâu  
- ~30% quay lại trong vòng 7 ngày trong giai đoạn làm nghiên cứu  
- Tín hiệu ban đầu cho thấy hành vi sử dụng lặp lại theo “đợt” (deadline), trong khi khả năng kiếm tiền và retention dài hạn vẫn đang được kiểm chứng  

6. THE ASK

Bọn em đang gọi 100–200 triệu VND vòng pre-seed để hoàn thiện MVP, tối ưu chi phí mỗi truy vấn và đạt 500–1,000 người dùng hoạt động trong 12 tháng tới, đồng thời kiểm chứng hành vi sử dụng lặp lại và mức độ sẵn sàng chi trả.
```


