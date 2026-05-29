# 02 — Group Problem Statement

Nhóm 3 người:

| Mã HV | Tên | Vai trò | Lát cắt |
|---|---|---|---|
| 2A202600778 | Trần Bá Đạt | HV VinAI Batch 02 | Tra cứu thông tin, lạc thông báo |
| 2A202600771 | Nguyễn Thành Đạt | HV VinAI Batch 02 | Đọc paper, viết progress log |
| 2A202600694 | Hoàng Lê Bách | HV VinAI Batch 02, có nền coding | Reuse code, debug, viết doc |

Trong bản nộp nhóm dưới đây, để phân biệt 2 bạn "Đạt", mình gọi:
- "Bá Đạt" = Trần Bá Đạt
- "Thành Đạt" = Nguyễn Thành Đạt (mình)
- "Bách" = Hoàng Lê Bách

## Phase 3 — Group Convergence

### Bước 3.1 — Trình bày top 3 (9 candidates)

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh |
|---|---|---|---|---|---|
| 1 | Bá Đạt | Tra cứu thông báo trainer trong Discord lab | HV VinAI Batch 02 | Đọc nhiều thread, không chắc message cuối | Workflow |
| 2 | Bá Đạt | Tổng hợp slide + notebook nhiều buổi để ôn lab | HV ôn cuối tuần | Lướt + viết lại summary | Workflow |
| 3 | Bá Đạt | Viết reflection sau lab | HV nộp bài | Nhớ lại phase đã làm | No AI / process fix |
| 4 | Thành Đạt | Tóm tắt paper AI 10-20 trang để quyết định có đọc kỹ không | HV đang research | Đọc skim + đánh giá relevance | Workflow |
| 5 | Thành Đạt | Hỏi lại thread Discord cũ để tìm câu trả lời của trainer | HV làm lab | Search keyword không trúng | Workflow |
| 6 | Thành Đạt | Viết weekly progress gửi mentor | HV có mentor | Không nhớ tuần đã làm gì | Workflow |
| 7 | Bách | Tìm lại code mẫu của trainer / bài cũ để reuse | HV lập trình | Search trong nhiều repo | Workflow / Rule |
| 8 | Bách | Debug error đã từng gặp nhưng quên fix | HV lập trình | Tra lỗi cũ trong note hoặc Stack Overflow | Workflow / Rule |
| 9 | Bách | Viết documentation cho lab nộp | HV nộp bài có code | Viết phần "vì sao chọn approach" | Workflow |

### Bước 3.2 — Gom trùng / cluster

| Cluster | Candidates included | Pattern chung | Ghi chú |
|---|---|---|---|
| A — Tra cứu / tìm lại thông tin có sẵn | #1 (Discord trainer), #5 (Discord thread cũ), #7 (code mẫu), #8 (error cũ) | "Thông tin từng có nhưng khó tìm lại" | Cluster mạnh nhất, 4/9 candidates |
| B — Tổng hợp / tóm tắt nhiều nguồn | #2 (slide ôn lab), #4 (paper summary) | Đọc nhiều nguồn → viết lại ngắn | 2 candidates |
| C — Viết update / reflection / doc | #3 (reflection), #6 (weekly progress), #9 (documentation) | Viết theo format có sẵn, mất công nhớ lại | 3 candidates |

Phát hiện: cluster A là cluster nhiều người chung pain nhất. Bài #5 của Thành Đạt và #1 của Bá Đạt gần như cùng problem; #7 và #8 của Bách khác kênh nhưng cùng pattern "tìm lại thứ từng có".

### Bước 3.3 — Shortlist

| Candidate | Vì sao vào shortlist | Rủi ro / điều chưa rõ |
|---|---|---|
| Cluster A — Tra cứu thông báo / quyết định trong Discord (gộp #1 và #5) | Nhiều người trong nhóm cùng đau, baseline thời gian có, có thể vẽ before/after, có thể so sánh R/W/A | Quyền access Discord API; tính chính xác khi trainer đính chính |
| Cluster B — Tóm tắt paper / tổng hợp tài liệu | AI có lợi thế rõ về ngôn ngữ | Metric "tóm tắt tốt" khó định nghĩa trong lab; risk hallucination cao |
| Cluster C — Viết weekly progress / reflection | Workflow rõ, mỗi tuần lặp lại | Reflection là phần cá nhân → boundary AI nhạy cảm; ít người trong nhóm cùng đau |

### Bước 3.4 — Score để đồng thuận

Thang 1-5.

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| A — Tra cứu Discord (gộp #1+#5+#7+#8) | 5 | 5 | 5 | 5 | 5 | 5 | 5 | 35 |
| B — Tóm tắt paper / tài liệu | 4 | 4 | 4 | 3 | 4 | 4 | 4 | 27 |
| C — Weekly progress / reflection | 4 | 4 | 3 | 3 | 4 | 3 | 3 | 24 |

**Candidate nhóm chọn:**

```text
Cluster A — Tra cứu thông báo / quyết định / tài nguyên có sẵn của lab VinAI.

Phiên bản hẹp lại để vừa thời gian lab:
"Tra cứu thông báo / đính chính của trainer trong Discord lab Batch 02"
(tập trung kênh announcements + batch-02 + q-and-a, không phải toàn bộ Discord).
```

**Vì sao chọn:**
- 3/3 thành viên cùng có evidence (Bá Đạt từng miss đính chính, Thành Đạt hay hỏi lại thread cũ, Bách dùng cùng pattern khi tìm code).
- Workflow lặp lại hằng tuần, có baseline 15-25 phút.
- Có metric đo được: thời gian tra cứu + số lần ping trainer trùng câu.
- So sánh R/W/A rõ: Rule (pin + FAQ), Workflow (retrieve + tóm tắt), Agent (tự hỏi-đáp như chatbot).

**Vì sao không chọn các candidate còn lại:**
- Cluster B (tóm tắt paper): metric "tóm tắt tốt" khó định nghĩa trong 4 tiếng lab; risk hallucination cao mà chưa có cách verify nhanh.
- Cluster C (reflection/progress): chính worksheet này cấm dùng AI viết thay reflection → boundary nhạy; pain mỗi người mỗi khác.
- Code reuse (#7) và debug error cũ (#8) thuộc cluster A nhưng nguồn data (repo cá nhân, Stack Overflow) khó index trong scope lab.

**Nếu có disagreement, nhóm xử lý thế nào:**
Bách ban đầu nghiêng về candidate #7 (tìm code mẫu) vì có thể demo nhanh. Nhóm hỏi: "Nếu mở rộng scope tới repo + Stack Overflow, có làm hết trong 4 tiếng không?" → không. Nhóm thống nhất giữ cluster A nhưng đổi tên candidate sang "tra cứu trong Discord lab" để có boundary rõ; Bách đồng ý sau khi thấy pattern giống nhau.

---

## Phase 4 — Quick Validation + Research

### Bước 4.1 — Quick validation

Vì lab giả định không thực sự chạy survey với 40 học viên, nhóm dùng 2 nguồn:

| Nguồn | Số người / mẫu | Tín hiệu xác nhận | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| Quick interview (3 bạn cùng Batch 02 ngoài nhóm) | 3 | 3/3 đều từng phải ping trainer hỏi lại deadline / format; 2/3 từng miss đính chính | 1 bạn nói "mình hay pin message nên ít bị" → có workaround nhưng vẫn 5-10 phút | Thu hẹp: pain rõ nhất là **đính chính trainer** (vì đính chính làm message cũ sai), không phải mọi loại thông báo |
| Quan sát Discord lab Batch 02 1 tuần gần nhất | ~50 message trong #announcements + #batch-02 | Có 3 đính chính trainer + 8 câu hỏi lặp lại của học viên về deadline/format | Một số đính chính trainer đã được pin → người chăm đọc sẽ thấy | Thêm boundary: tool chỉ retrieve, ưu tiên message **mới nhất cùng topic** để xử lý case đính chính |

**Insight sau validation:**

```text
Pain không phải "Discord khó search nói chung", mà là "khi trainer đính chính, message cũ vẫn nổi
trong kết quả search, khiến học viên đọc trúng phiên bản sai và submit nhầm". Workflow tool phải
ưu tiên message mới nhất theo topic và luôn cite link gốc để học viên tự verify.
```

### Bước 4.2 — Research giải pháp đã có

| Nguồn / tool / case | Link | Họ giải quyết phần nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Discord built-in search | https://support.discord.com/hc/en-us/articles/115000468588-Using-Search | Search keyword trong server/channel | Có sẵn, không cần build | Không hiểu ngữ nghĩa, không ưu tiên message mới hơn cùng topic | Rule keyword search không đủ cho case đính chính |
| Discord Forum Channels | https://support.discord.com/hc/en-us/articles/6208479917079-Forum-Channels-FAQ | Tổ chức thread theo topic | Giảm bớt việc trôi message | Vẫn phải search trong từng forum; trainer phải đổi cách post | Có thể bổ sung cho Rule nhưng cần thay đổi quy ước batch |
| Slack AI recap & search | https://slack.com/help/articles/25076892548883-Guide-to-Slack-AI | Tóm tắt + search có ngữ nghĩa | Đã chứng minh pattern "AI summary + cite source" hoạt động | Khác platform; Discord chưa có tính năng tương đương | Pattern "tóm tắt + cite link gốc" đáng học |
| Bot kiểu Glassfrog / Needle in Discord (qua webhook + RAG) | https://needle-ai.com/ (ví dụ RAG-as-a-service) | Index doc/Discord rồi trả lời có cite | Có sẵn pattern RAG cho Discord | Cần permission bot, cần index lại định kỳ; nhiều tool tính phí | Khả thi về mặt kỹ thuật; vấn đề là quyền + chi phí |

**Research takeaway:**

```text
Không cần build agent đa năng. Pattern hợp lý: RAG đơn giản trên 2-3 channel chính, trả về top-K
message + tóm tắt + link gốc. Ưu tiên message mới nhất cùng topic (xử lý case đính chính). Học
viên click link để verify. Đây là Workflow, không phải Agent.
```

---

## Phase 5 — Workflow + Problem Statement

### Bước 5.1 — Current workflow bản nhóm

File Mermaid: `02-group-problem-statement-workflow-current.mmd`

```text
CURRENT STATE — 7 bước, 15-25 phút mỗi lần tra cứu

[1 HV xác định cần tra cứu thông tin: 0.5']
→ [2 Đoán channel (announcements / batch-02 / q-and-a): 2']
→ [3 Search keyword Discord: 3']
→ [4 Lọc thread, đọc 5-10 message: 8']                <-- bottleneck
→ [5 Không chắc phiên bản nào là cuối → ping trainer/bạn: 5']  <-- bottleneck phụ
→ [6 Chờ phản hồi (có khi đến 1-2 ngày): 5'+ ]
→ [7 Apply thông tin vào lab: 2']
```

| Bước | Actor | Input | Output | Thời gian/tần suất | Ghi chú |
|---|---|---|---|---|---|
| 1 | HV | Câu hỏi trong đầu | Quyết định tra cứu | 0.5' | 3-4 lần/tuần/HV |
| 2 | HV | Tên các channel | Channel chọn | 2' | Hay đoán sai channel |
| 3 | HV | Keyword | Danh sách message | 3' | Discord search không hiểu ngữ nghĩa |
| 4 | HV | Message list | Phiên bản ứng viên | 8' | **Bottleneck**: phải đọc, không chắc |
| 5 | HV → trainer | Câu hỏi | Phản hồi (sau X giờ) | 5' viết + chờ | Phụ thuộc trainer online |
| 6 | Trainer | Câu hỏi | Câu trả lời | Biến thiên | Trainer bị ping nhiều câu trùng |
| 7 | HV | Câu trả lời cuối | Apply vào lab | 2' | |

**Bottleneck chính:** bước 4-5. Khi trainer đính chính trong message mới, search vẫn trả về cả bản cũ → HV đọc trúng bản sai.

### Bước 5.2 — Future workflow bản nhóm

File Mermaid: `02-group-problem-statement-workflow-future.mmd`

```text
FUTURE STATE — 5 bước, dưới 6 phút mỗi lần tra cứu

[1 HV hỏi 1 câu trong tool (qua bot Discord hoặc web nội bộ): 0.5']
→ [2 Rule: lấy snapshot 2-3 channel chính (refresh mỗi 6h): tự động, 0']
→ [3 AI workflow: retrieve top 5 message liên quan
       + ưu tiên message mới nhất cùng topic
       + tóm tắt ngắn + cite link gốc: 0.5']
→ [4 HV đọc tóm tắt + click link gốc verify: 3']     <-- human boundary
→ [5 Apply vào lab: 2']

Boundary:
- AI chỉ retrieve + tóm tắt từ message đã có. KHÔNG tự trả lời câu hỏi mới.
- AI KHÔNG truy cập DM / channel instructor-only.
- Mỗi câu trả lời phải có ít nhất 1 link gốc để HV verify.
- Nếu confidence < threshold → AI nói "không chắc, hỏi trainer ở channel X".

Fallback:
- AI sai / tóm tắt nhạt → HV vẫn có link gốc, đọc trực tiếp như cũ.
- Trainer đính chính sau → snapshot tiếp theo (≤ 6h) sẽ ưu tiên message mới.
- Nếu tool die → quay về workflow current, không chặn HV.
```

| Bước | Actor | Input | Output | Thời gian/tần suất | Ghi chú |
|---|---|---|---|---|---|
| 1 | HV | Câu hỏi | Query | 0.5' | |
| 2 | Rule/script | Discord API | Snapshot 2-3 channel | Tự động, 6h/lần | Không người |
| 3 | AI (RAG) | Query + snapshot | Top 5 message + tóm tắt + link | 0.5' | Ưu tiên recency cùng topic |
| 4 | HV | Tóm tắt + link | Confirm nội dung | 3' | **Human boundary** |
| 5 | HV | Nội dung verified | Apply vào lab | 2' | |

#### Before/after impact

| Metric | Trước | Sau kỳ vọng | Ghi chú |
|---|---:|---:|---|
| Số bước HV thực hiện | 7 | 4 (HV) + 1 tự động | Bước 2 chuyển sang tự động |
| Tổng thời gian / lần tra cứu | 15-25 phút | < 6 phút | Target chính |
| Số bước thủ công | 6/7 | 4/5 | HV vẫn verify + apply |
| Bottleneck chính | Đọc thread + chờ trainer | HV verify link gốc | Boundary chấp nhận được |
| Risk mới | Có thể đọc trúng bản trainer đã sửa | AI tóm tắt sai / outdated snapshot | Bù bằng cite link + refresh 6h |

### Bước 5.3 — Problem Statement v0

| Field | Nội dung |
|---|---|
| **Actor** | Học viên VinAI Batch 02 đang làm lab, cần xác nhận thông tin trainer đã thông báo. |
| **Workflow** | HV đoán channel → search keyword Discord → đọc 5-10 message → ping trainer khi không chắc → chờ phản hồi → apply. |
| **Bottleneck** | Đọc thread + không chắc phiên bản đính chính nào là cuối → phải ping trainer. Mỗi lần 8-13 phút và phụ thuộc trainer online. |
| **Impact** | 15-25 phút/lần × 3-4 lần/tuần/HV. ~40 HV trong batch → 30-60 giờ/tuần toàn batch. Trainer bị ping trùng câu hỏi. Đã có case submit nhầm vì miss đính chính. |
| **Success Metric** | Thời gian tra cứu median < 5 phút. Số ping trainer trùng topic deadline/format/đính chính / tuần giảm ≥ 50%. Không có case "submit nhầm vì đọc bản cũ" trong 4 tuần pilot. |
| **Boundary** | Chỉ retrieve message đã có; không tự trả lời câu hỏi mới; không truy cập DM / channel instructor-only; mọi câu trả lời có link gốc; nếu confidence thấp → suggest hỏi trainer. |

---

## Phase 6 — Rule / Workflow / Agent + Decision

### Bước 6.0 — Ma trận độ phù hợp

| | Độ mơ hồ thấp | Độ mơ hồ cao |
|---|---|---|
| **Độ phức tạp thấp** | Rule / dashboard đủ | Workflow có AI 1 bước có thể đủ |
| **Độ phức tạp cao** | Workflow điều phối | Agent có thể phù hợp (cần boundary chặt) |

**Bài toán nhóm nằm ở:** Độ phức tạp thấp-trung bình + Độ mơ hồ trung bình.

Vì sao:
- Độ phức tạp: 1 query → retrieve → tóm tắt → trả về. Không nhiều nhánh.
- Độ mơ hồ: câu hỏi của HV có thể diễn đạt khác nhau (vd "hạn nộp lab 02?" vs "bao giờ cuối tuần này"), nên Rule keyword không đủ.
- AI không cần tự quyết bước tiếp theo.

→ Workflow hỗ trợ 1-2 bước AI là phù hợp. Agent là quá mức.

### Bước 6.1 — So sánh Rule / Workflow / Agent

| Mức | Phương án cho bài toán nhóm | Khi nào đủ | Rủi ro | Chọn? |
|---|---|---|---|---|
| **Rule** | Pin thông báo + FAQ file trong repo + 1 forum channel cho deadline | Đủ nếu trainer kỷ luật pin và HV chịu đọc forum | Phụ thuộc kỷ luật người; vẫn không xử lý ngữ nghĩa (HV dùng từ khác); đính chính vẫn lẫn lộn | Dùng kết hợp, không đủ một mình |
| **Workflow** | Bot Discord hoặc web nội bộ: index 2-3 channel → retrieve top-K + ưu tiên recency cùng topic → tóm tắt + cite link → HV verify | Hợp vì đường đi tuyến tính, AI chỉ làm 1 bước ngôn ngữ | Tóm tắt sai, snapshot stale; HV lười click link gốc | **Chọn** |
| **Agent** | Chatbot tự trả lời + tự quyết khi nào ping trainer + tự cập nhật FAQ | Chỉ cần nếu cần tự lập kế hoạch / nhiều tool / nhiều bước phụ thuộc | Quá rộng; risk hallucinate câu trả lời trainer chưa từng nói; quyền access lớn | Không chọn |

Hỏi kỹ:
- Rule giải được 70-80%? — Không. Pin + FAQ giúp ~40-50% nhưng case đính chính + ngữ nghĩa vẫn lọt.
- Workflow đủ? — Có. AI chỉ làm bước rank + tóm tắt + cite. HV vẫn verify.
- Cần Agent? — Không. Không có nhiều nhánh, không cần tự lập kế hoạch.
- Nếu AI sai, ai phát hiện và sửa? — HV (qua bước verify link gốc). Trainer nếu HV ping lại do confidence thấp.
- Có thể hạ mức? — Có. Nếu pilot cho thấy 80% câu hỏi Rule + Pin xử lý được, có thể giữ Rule cho phần đó, Workflow cho phần còn lại.

**Mức chọn:**

```text
Workflow.
(Có dùng Rule cho bước snapshot + pin thông báo; không dùng Agent.)
```

**Vì sao chọn:**
- Workflow tuyến tính: query → retrieve → rank → tóm tắt → cite → HV verify.
- AI chỉ hỗ trợ 1 bước ngôn ngữ (retrieve theo ngữ nghĩa + tóm tắt + ưu tiên recency).
- HV vẫn là người verify cuối cùng → risk kiểm soát được.
- Có fallback rõ (cite link gốc, suggest hỏi trainer).

**Vì sao không chọn mức đơn giản hơn (Rule một mình):**
- Rule keyword không xử lý được câu hỏi diễn đạt khác.
- Pin + FAQ phụ thuộc kỷ luật trainer + HV; không xử lý đính chính nhanh.
- Vẫn để lọt 50%+ trường hợp đính chính → vẫn ping trainer.

### Bước 6.2 — Problem Statement v1

| Field | Nội dung |
|---|---|
| **Actor** | Học viên VinAI Batch 02 đang làm lab, cần xác nhận thông tin trainer đã thông báo. |
| **Workflow** | HV gửi câu hỏi → tool snapshot 2-3 channel chính (Rule, 6h/lần) → AI retrieve top 5 message + ưu tiên recency cùng topic + tóm tắt + cite link → HV click link verify → apply vào lab. |
| **Bottleneck** | (Cũ) đọc thread + ping trainer cho đính chính. (Mới) HV cần click link verify. |
| **Impact** | Mục tiêu: 15-25' → dưới 6' / lần; giảm ≥ 50% ping trainer trùng topic deadline/format/đính chính. |
| **Success Metric** | (1) Thời gian tra cứu median < 5' đo từ log tool. (2) Số ping trainer trùng câu/tuần giảm ≥ 50% sau 4 tuần. (3) 0 case "submit nhầm bản cũ" trong 4 tuần pilot. |
| **Boundary** | Chỉ retrieve message đã có; không tự trả lời câu hỏi mới; không truy cập DM/instructor-only; mọi câu trả lời cite ít nhất 1 link gốc; confidence < threshold → suggest hỏi trainer. |
| **AI intervention point** | Sau khi snapshot có sẵn (đầu vào structured), trước bước HV verify. AI chỉ rank + tóm tắt + cite. |
| **Mức chọn** | Workflow (Rule cho snapshot + ranking recency; AI cho semantic retrieval + tóm tắt). |
| **Rủi ro & người thật kiểm tra** | Risk: tóm tắt sai, snapshot stale, HV lười click link gốc, AI hallucinate khi không có câu trả lời rõ. Người kiểm: HV verify mỗi lần; trainer reviewer ngẫu nhiên 10 câu/tuần trong pilot; có channel báo lỗi. |

### Bước 6.3 — Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú |
|---|---|---|
| Actor và workflow đã rõ chưa? | Yes | HV Batch 02; workflow 5 bước rõ |
| Baseline và success metric đã đo được chưa? | Yes (baseline tự khai) / Not Yet (cần đo log thật) | 15-25' từ self-report; pilot cần đo log tool |
| Có data/input đủ dùng chưa? | Not Yet | Cần xin quyền bot Discord cho 2 channel chính |
| Nếu AI sai, hậu quả có chấp nhận được không? | Yes | HV verify link gốc; risk thấp vì cite source |
| Có người review/owner vận hành không? | Yes | Bá Đạt làm pilot owner; 1 trainer review 10 câu/tuần |
| Có cách non-AI đơn giản hơn không? | Có một phần | Pin + FAQ + Forum channel — giải 40-50%, không xử lý ngữ nghĩa + đính chính |

**Decision:**

```text
Go với scope pilot nhỏ.
```

**Lý do:**
- Problem rõ, workflow rõ, metric đo được.
- Có cả Non-AI component (Rule snapshot + pin) và AI component (semantic retrieve + tóm tắt).
- AI chỉ ở một bước, không ôm cả workflow.
- HV verify trước khi apply → risk thấp.
- Pilot scope nhỏ → nếu fail dễ dừng.

**Pilot nhỏ nhất:**

```text
- Index 2 channel: #announcements + #batch-02-q-and-a (30 message gần nhất).
- Snapshot refresh thủ công 1 lần/ngày trong 2 tuần đầu.
- Triển khai dưới dạng web nội bộ (không cần Discord bot ngay) → HV truy cập 1 URL, gõ câu hỏi.
- Test với 5-7 HV tình nguyện, 2 tuần.
- Đo: thời gian tra cứu, số ping trainer trùng, số case "submit nhầm bản cũ".
- 1 trainer review ngẫu nhiên 10 câu trả lời/tuần để chấm chất lượng.
```

**Nếu Not Yet, cần validate gì trước:** (đã ghi cho phòng hờ)
- Quyền access Discord API / bot.
- Baseline ping trainer trùng (đo 1 tuần trước pilot).
- Trainer có sẵn sàng review 10 câu/tuần không.

**Nếu No-Go, nên làm gì thay AI:**
- Quy ước batch: trainer luôn pin đính chính + chốt deadline trong 1 channel duy nhất.
- 1 FAQ file Markdown trong repo lớp, cập nhật cuối mỗi tuần.
- Forum channel theo từng lab.
