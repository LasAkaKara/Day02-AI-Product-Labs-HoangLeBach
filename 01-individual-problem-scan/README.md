# Phase 1 - Scan rộng

Mình scan 8 problems từ trải nghiệm thật khi học VinAI Batch 02, làm lab có code, làm việc nhóm và theo dõi thông tin trong Discord / tài liệu khóa học.

| # | Lăng kính | Problem quan sát được | Ai đang đau? | Dấu hiệu |
| - | --- | --- | --- | --- |
| 1 | Lặp lại / Tốn thời gian | Tìm lại code mẫu của trainer hoặc bài lab cũ để reuse | Mình + HV có làm lab coding | Nhớ là đã từng thấy đoạn code tương tự nhưng không nhớ nằm ở repo/notebook nào; mỗi lần tìm mất khoảng 10-20 phút |
| 2 | Tốn thời gian | Debug lại error đã từng gặp nhưng quên fix | Mình + HV lập trình | Gặp lại lỗi cũ nhưng vẫn phải search note/Stack Overflow từ đầu; mỗi lỗi có thể mất 15-30 phút để mò lại |
| 3 | Lặp lại | Viết documentation / README cho lab nộp | Mình + HV nộp bài có code | Code chạy được nhưng phần “vì sao chọn approach”, cách chạy, limitation mất 30-45 phút để viết lại cho rõ |
| 4 | Pain từ người khác | Mentor/TA phải chấm nhiều bài code nhưng khó nhìn nhanh bài nào thiếu phần quan trọng | Mentor, TA, trainer review bài | Mỗi bài phải mở repo, đọc README, skim code, kiểm tra output/reflection; nhiều lỗi lặp lại như thiếu cách chạy, thiếu giải thích approach |
| 5 | Collaboration / Pain từ người khác | Nhóm khó gom nhiều ý tưởng cá nhân thành một candidate problem chung | Nhóm 3-4 HV trong lab | Mỗi người pitch top 3 nhưng note rời rạc; dễ chọn theo cảm tính hoặc nhảy sang solution trước khi thống nhất problem |
| 6 | Research / AI có thể tốt hơn | Tìm existing solutions/tools cho problem nhóm nhưng dễ chọn nguồn hời hợt | Mình + nhóm làm Phase 4 validation/research | Google nhiều link nhưng khó biết nguồn nào đáng tin; dễ ghi tool cho có mà chưa rút được bài học cho problem nhóm |
| 7 | Lặp lại / Tốn thời gian | Theo dõi mình đã làm gì trong tuần để viết progress/reflection | Mình + HV có mentor hoặc nhiều lab song song | Cuối tuần phải lục lại Discord, Git commit, note cá nhân để nhớ mình đã làm gì; mỗi lần 20-30 phút |
| 8 | Pain từ người khác / Course workflow | Học viên miss thông báo hoặc đính chính của trainer trong Discord | HV VinAI Batch 02 + trainer bị hỏi lại | Search keyword không trúng hoặc đọc nhầm message cũ; mỗi lần tra cứu 15-25 phút; trainer/bạn phải trả lời lại câu trùng |


# Phase 2 - Chọn Top 3 + Problem Cards

## Chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
| --- | --- | --- | --- |
| 1 | Tìm lại code mẫu của trainer hoặc bài lab cũ để reuse (#1) | Actor rõ, workflow dễ vẽ, bottleneck nằm ở bước search nhiều repo/notebook. Impact đo được bằng thời gian tìm code mỗi lần. | Code nằm rải rác, chưa chắc dễ index chính xác. |
| 2 | Debug lại error đã từng gặp nhưng quên fix (#2) | Pain rõ, mỗi lỗi có thể tốn nhiều thời gian. Workflow cụ thể: gặp lỗi → search → thử fix → chạy lại. Metric đo được bằng thời gian debug. | Nếu không có bug log/note cũ thì dữ liệu đầu vào yếu. |
| 3 | Viết documentation cho lab nộp (#3) | Việc lặp lại sau mỗi lab có code, workflow rõ: code xong → nhớ lại approach → viết README → giải thích cách chạy/limitation. Impact đo được bằng thời gian viết doc và số câu hỏi reviewer hỏi lại. | Khó đo “documentation tốt”; AI có thể bịa lý do nếu mình không ghi lại decision trong lúc làm. |


## Problem Card #1 - Tìm lại code mẫu của trainer hoặc bài lab cũ để reuse

**Problem 1 câu:**
Khi làm lab coding, học viên mất 10-20 phút mỗi lần để tìm lại code mẫu hoặc bài lab cũ đã từng thấy, vì code nằm rải rác trong nhiều repo, notebook hoặc tài liệu khác nhau.

**Actor:**
Mình và các học viên VinAI Batch 02 đang làm lab có code.

**Thời điểm / bối cảnh:**
Khi đang làm bài lab mới, gặp một phần code quen thuộc như data loading, training loop, evaluation, visualization hoặc config, và muốn reuse từ bài cũ/trainer demo.

**Current workflow:**

```text
1. Nhớ mang máng là trainer từng demo đoạn code tương tự
2. Mở lại repo / notebook / Discord / tài liệu cũ
3. Search keyword theo trí nhớ
4. Mở nhiều file để skim thủ công
5. Copy đoạn code gần đúng
6. Sửa lại cho phù hợp với bài lab hiện tại
7. Chạy thử và debug nếu không khớp
```

**Bottleneck:**
Bước 3-4 - search và skim nhiều file thủ công. Mỗi lần mất khoảng 10-20 phút, đặc biệt khi không nhớ chính xác keyword hoặc file chứa code.

**Impact:**
Làm chậm tiến độ lab, dễ làm lại từ đầu dù đã có code tương tự. Nếu gặp 2-3 lần trong một lab, tổng thời gian mất có thể lên tới 30-60 phút chỉ để tìm lại reference.

**Success metric:**
Giảm thời gian tìm lại code mẫu từ 10-20 phút xuống dưới 3-5 phút/lần, và học viên tìm được đúng file/đoạn code cần dùng mà không phải mở quá nhiều notebook.

**Non-AI alternative:**
Tạo index thủ công cho các bài lab: tên bài, chủ đề, link file, đoạn code quan trọng. Cách này ít rủi ro nhưng cần duy trì đều và chỉ hiệu quả nếu mọi người đặt tên/tag tốt.

**AI hypothesis:**
AI có thể hỗ trợ semantic search trên repo/notebook: học viên mô tả bằng ngôn ngữ tự nhiên, AI gợi ý file/đoạn code liên quan và tóm tắt đoạn đó dùng để làm gì. Học viên vẫn phải đọc code và tự quyết định có reuse không.

**Quick gut:**
Workflow.

### Draft current workflow

```text
CURRENT STATE - 10-20 phút/lần

[Nhớ có code tương tự: 1']
→ [Mở repo/notebook/Discord: 2-3']
→ [Search keyword thủ công: 3-5']
→ [Skim nhiều file: 5-10']  <-- bottleneck
→ [Copy code gần đúng: 1']
→ [Sửa và chạy thử: 3-5']
```

### Draft future workflow

```text
FUTURE STATE - 3-5 phút/lần

[Nhập mô tả cần tìm: 30s]
→ [Search/index trả về file + đoạn code liên quan: 1']
→ [AI tóm tắt đoạn code và context dùng: 1']
→ [Học viên kiểm code và copy phần cần dùng: 1-2']  <-- human boundary
→ [Chạy thử trong lab hiện tại: 1']

Fallback: nếu kết quả search sai → quay lại search thủ công hoặc hỏi trainer/bạn học.
```

---

## Problem Card #2 - Debug lại error đã từng gặp nhưng quên fix

**Problem 1 câu:**
Khi gặp lại một lỗi lập trình đã từng xử lý, học viên vẫn mất 15-30 phút để search lại note, Stack Overflow hoặc mò lại cách fix vì không có nơi lưu bug-fix theo context lab.

**Actor:**
Mình và học viên lập trình trong các bài lab AI/ML.

**Thời điểm / bối cảnh:**
Trong lúc chạy notebook/script, gặp lỗi quen thuộc như mismatch tensor shape, CUDA/device error, package version conflict, path sai, hoặc lỗi data format.

**Current workflow:**

```text
1. Chạy code và gặp error
2. Nhớ là lỗi này đã từng gặp trước đó
3. Search lại trong note cá nhân / browser history / Stack Overflow / Discord
4. Đọc nhiều kết quả để xem cái nào giống context hiện tại
5. Thử một hoặc nhiều cách fix
6. Chạy lại code
7. Nếu chưa được thì tiếp tục search/debug
```

**Bottleneck:**
Bước 3-5 - tìm lại đúng cách fix theo đúng context. Lỗi có thể giống message nhưng khác nguyên nhân, nên dễ thử sai nhiều lần.

**Impact:**
Mỗi lỗi lặp lại có thể tốn 15-30 phút. Ngoài mất thời gian, việc debug lại từ đầu làm đứt mạch học và khiến học viên khó tập trung vào nội dung chính của lab.

**Success metric:**
Giảm thời gian xử lý các lỗi đã từng gặp từ 15-30 phút xuống dưới 5-10 phút/lần, với điều kiện cách fix được gợi ý phải có context và nguồn từ log/note cũ.

**Non-AI alternative:**
Tạo bug log dạng bảng gồm: error message, bài lab gặp lỗi, nguyên nhân, cách fix, link commit/notebook. Cách này rõ ràng và ít rủi ro, nhưng học viên phải nhớ ghi lại sau mỗi lần debug.

**AI hypothesis:**
AI có thể đọc error message hiện tại, tìm trong bug log/note cũ các lỗi tương tự, rồi gợi ý 2-3 hướng fix kèm lý do. AI không tự sửa code; học viên vẫn kiểm tra nguyên nhân, chọn fix và chạy lại.

**Quick gut:**
Workflow.

### Draft current workflow

```text
CURRENT STATE - 15-30 phút/lỗi

[Chạy code gặp error: 1']
→ [Đọc error message: 2-3']
→ [Nhớ đã gặp nhưng không nhớ fix: 1']
→ [Search note/Google/Discord: 5-10']  <-- bottleneck
→ [Thử fix 1: 5']
→ [Chạy lại: 2']
→ [Nếu sai, tiếp tục thử fix khác: 5-10']
```

### Draft future workflow

```text
FUTURE STATE - 5-10 phút/lỗi

[Paste error + context lab: 1']
→ [Hệ thống tìm bug log/note tương tự: 1']
→ [AI gợi ý nguyên nhân khả dĩ + cách fix: 1-2']
→ [Học viên chọn fix và sửa code: 2-4']  <-- human boundary
→ [Chạy lại để verify: 1-2']

Fallback: nếu bug chưa có trong log hoặc AI gợi ý sai → debug thủ công và ghi lại bug mới vào log.
```

---

## Problem Card #3 - Viết documentation cho lab nộp

**Problem 1 câu:**
Sau khi code lab chạy được, học viên vẫn mất 30-45 phút để viết README/documentation vì phải nhớ lại approach, cách chạy, kết quả, limitation và giải thích sao cho reviewer hiểu.

**Actor:**
Mình và học viên VinAI Batch 02 nộp bài lab có code; gián tiếp còn có mentor/TA/reviewer đọc bài.

**Thời điểm / bối cảnh:**
Cuối mỗi bài lab hoặc project nhỏ, sau khi code đã chạy, cần viết README để nộp bài: mô tả cách chạy, cấu trúc repo, approach, kết quả, limitation và reflection ngắn.

**Current workflow:**

```text
1. Code xong và kiểm tra output
2. Mở README trống hoặc template cũ
3. Nhớ lại mình đã làm những bước nào
4. Viết cách setup/chạy code
5. Viết approach, kết quả, limitation
6. Đọc lại để xem reviewer có hiểu không
7. Sửa format và nộp repo
```

**Bottleneck:**
Bước 3-5 - biến quá trình làm code thành giải thích rõ ràng. Dù code đã chạy, học viên vẫn phải nhớ lại decision, lỗi đã gặp, vì sao chọn approach và limitation.

**Impact:**
Mỗi lab mất thêm 30-45 phút để viết documentation. Nếu viết thiếu, reviewer/TA phải hỏi lại hoặc khó đánh giá đúng bài làm. Điều này cũng làm học viên dễ nộp bài có code nhưng thiếu phần giải thích.

**Success metric:**
Giảm thời gian viết README từ 30-45 phút xuống dưới 15-20 phút, đồng thời giảm số câu hỏi reviewer phải hỏi lại về cách chạy, approach hoặc limitation.

**Non-AI alternative:**
Dùng README template cố định + checklist trước khi nộp, ví dụ: setup, command chạy, data, approach, result, limitation. Cách này có thể giải quyết phần format nhưng chưa giúp viết lại reasoning từ quá trình làm bài.

**AI hypothesis:**
AI có thể tạo draft README từ template, code structure, commit/note ngắn và output mẫu. Học viên vẫn phải kiểm tra lại nội dung, sửa phần approach/limitation và đảm bảo AI không bịa lý do hoặc kết quả.

**Quick gut:**
Workflow.

### Draft current workflow

```text
CURRENT STATE - 30-45 phút/lab

[Code chạy được: 0']
→ [Mở README/template: 2']
→ [Nhớ lại approach đã làm: 10-15']  <-- bottleneck
→ [Viết cách chạy + cấu trúc repo: 8-10']
→ [Viết result + limitation: 8-10']
→ [Review lại cho rõ: 5-10']
→ [Format và nộp: 2-3']
```

### Draft future workflow

```text
FUTURE STATE - 15-20 phút/lab

[Học viên cung cấp template + note ngắn + output chính: 3-5']
→ [AI draft README theo format: 2-3']
→ [Học viên kiểm từng phần: cách chạy, approach, result: 5-7']  <-- human boundary
→ [Học viên sửa limitation/reflection bằng hiểu biết thật: 3-5']
→ [Format và nộp: 1-2']

Fallback: nếu AI draft sai hoặc bịa reasoning → chỉ giữ template/checklist, học viên tự viết lại nội dung chính.
```

---

## Card tôi muốn pitch nhất

```text
Viết documentation cho lab nộp.
```

**Vì sao:**
Bài này có workflow rõ, xảy ra lặp lại sau mỗi lab có code, actor cụ thể và impact đo được bằng thời gian viết README cũng như số câu hỏi reviewer phải hỏi lại. Ngoài ra, bài này không chỉ đau cho học viên mà còn ảnh hưởng đến mentor/TA khi review bài. Scope cũng vừa đủ cho lab: có thể so sánh template thường, workflow có AI draft, và agent tự động toàn phần.

**Câu hỏi tôi muốn nhóm challenge:**

```text
Metric “README tốt” nên đo bằng gì ngoài thời gian viết?
AI nên được phép draft phần nào, và phần nào bắt buộc học viên phải tự viết để tránh bịa approach/limitation?
```
