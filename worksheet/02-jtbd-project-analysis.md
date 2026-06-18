---
artifact: 02 — JTBD Project Analysis
bai-tap: Lab 2 — Dùng JTBD để soi lại dự án nhóm
format: Theo nhóm dự án → share trong bàn → chốt hypothesis cuối
time: 25 phút trên lớp
nop-cuoi: Có — đây là file nộp cuối của Lab 2
companion-reference: Strategyn_JTBD_Playbook.pdf (giảng viên gửi kèm)
---

# Lab 2 — JTBD Project Analysis / Dùng JTBD để soi lại dự án nhóm

**Tên dự án / sản phẩm:** AI Code Review Assistant (Trợ lý AI tự động đánh giá Pull Request)  

> Đây là **file duy nhất** của Lab 2.  
> File này đồng thời đóng vai trò:
>
> - guide từng bước,
> - worksheet để điền trực tiếp,
> - và file nộp cuối cho người chấm.

Mục tiêu của bài này không phải brainstorm thêm thật nhiều tính năng AI.
Mục tiêu là:

1. **xác định người dùng thực sự đang cố hoàn thành job gì**
2. **hiểu họ đang dùng giải pháp nào để hoàn thành job đó hôm nay**
3. **chỉ ra AI nên chen vào đúng bước nào trong workflow**
4. **viết ra product hypothesis và assumption còn phải validate**

Quy tắc xuyên suốt: **không rõ job thì đừng bàn feature.**

---

## Cần mở song song 2 thứ

1. **File này** — để điền trực tiếp
2. **`Strategyn_JTBD_Playbook.pdf`** — giảng viên gửi kèm

### Cách dùng playbook cho đúng

Bạn **không cần đọc hết 48 trang**.  
Trong bài này, playbook chủ yếu dùng để tra 4 thứ:

1. **Cách nhìn thị trường qua JTBD lens**
2. **`Job executor` là ai**
3. **Cách viết `job statement`: `verb + object + contextual clarifier`**
4. **8 bước của `job map`**:
   `define -> locate -> prepare -> confirm -> execute -> monitor -> modify -> conclude`

### 2 chương nên mở nhiều nhất

- **Chapter 2 — Define Your Market**
- **Chapter 3 — Build Your Job Map**

> Dùng playbook để **tra framework và ví dụ**.  
> Dùng file này để **làm bài và chốt output**.

---

## Đầu ra bắt buộc

Người chấm cần thấy đủ 6 phần trong chính file này:

1. **`Project slice` + market context**
2. **`Job executor` + `core JTBD`**
3. **3 `job stories`**
4. **`JTBD lite map` + pain points**
5. **`AI leverage point` + `product hypothesis`**
6. **`Assumptions to validate` + verdict cuối sau thảo luận**

Nếu thiếu một trong sáu phần trên, bài sẽ bị xem là chưa hoàn chỉnh.

---

## Cách làm trong lớp (25 phút)

```text
3'  Chốt 1 lát cắt cụ thể của dự án
7'  Viết market context + job executor + core JTBD
6'  Viết 3 job stories + current alternatives
6'  Điền JTBD lite map + AI leverage point + hypothesis
3'  Share trong bàn và sửa version cuối
```

> Nếu dự án làm theo nhóm, cả nhóm có thể thảo luận chung.  
> Nhưng file này vẫn nên có **version chốt rõ ràng** của người nộp.

---

## Bước 0 — Khoanh đúng 1 lát cắt của dự án

Phần lớn dự án nhóm viết quá rộng ở bước này, rồi sau đó mọi thứ mơ hồ theo.

### Khoanh đúng 1 lát cắt theo 4 điểm

- [ ] **1 nhóm người dùng chính**
- [ ] **1 hoàn cảnh / tình huống rõ**
- [ ] **1 job cốt lõi**
- [ ] **1 workflow đủ cụ thể để vẽ ra được**

### Điền nhanh trước khi làm

- **Dự án của nhóm tôi là:** Trợ lý AI tích hợp vào GitHub/GitLab để review code tự động.
- **Lát cắt tôi chọn để phân tích hôm nay là:** Giúp Senior Developer / Tech Lead review các Pull Request (PR) nhanh và chuẩn xác hơn trước khi merge.
- **Vì sao tôi chọn lát cắt này:**  
  > Vì bước review PR hiện tại là nút thắt cổ chai (bottleneck) lớn nhất của team dev, tốn rất nhiều thời gian và dễ lọt bug do người review bị mệt mỏi (cognitive overload).

### Viết quá rộng vs viết sắc hơn

| Viết quá rộng | Viết sắc hơn |
|---|---|
| Giúp SME dùng AI để marketing | Giúp chủ shop online phản hồi câu hỏi trước mua hàng nhanh và nhất quán trong giờ cao điểm |
| Dùng AI để làm slide | Tạo bản nháp deck nội bộ mạch lạc cho buổi họp gấp trong thời gian rất ngắn |
| AI cho tuyển dụng | Giúp recruiter sàng lọc CV đầu vào nhanh hơn trước vòng gọi sơ bộ |

> Nếu bạn không mô tả được **một hoàn cảnh cụ thể**, khả năng cao bạn đang viết quá rộng.

---

## Bước 1 — Viết `Project Snapshot`

### Tóm tắt dự án trong 3 dòng

1. **Nhóm tôi đang nghĩ mình đang giải quyết vấn đề gì?**  
   > Quá trình code review thủ công tốn quá nhiều thời gian của nhân sự cấp cao và dễ bị sót lỗi (human error).

2. **Người dùng chính hiện nhóm đang nhắm tới là ai?**  
   > Senior Developer hoặc Tech Lead (những người được giao nhiệm vụ duyệt code/PR).

3. **Hiện tại người dùng đó đang giải quyết vấn đề này bằng cách nào?**  
   > Đọc code bằng mắt thường trên GitHub/GitLab, chạy test cục bộ, hoặc thỉnh thoảng copy từng đoạn nhỏ thả vào ChatGPT.

---

## Bước 2 — Viết `Market Context`

Ở đây chưa cần solution. Chỉ cần bối cảnh thị trường đủ để hiểu:
**ai đang gặp chuyện gì, trong hoàn cảnh nào, và vì sao bây giờ đáng giải.**

### Trả lời 4 câu ngắn

1. **Ai đang gặp vấn đề này?**  
   > Tech Lead / Senior Developer tại các đội dev bận rộn.

2. **Vấn đề xuất hiện trong hoàn cảnh nào?**  
   > Khi có quá nhiều PR được mở mỗi ngày, sát giờ release, khiến người review bị quá tải context.

3. **Hiện tại họ đang dùng giải pháp thay thế nào?**  
   > Review thủ công (đọc diff), tích hợp SonarQube (phân tích tĩnh) hoặc CI/CD cơ bản.

4. **Vì sao đây là thời điểm đáng giải?**  
   > Context window của các mô hình LLM đã đủ lớn để "hiểu" cấu trúc toàn bộ codebase thay vì chỉ vài dòng code rời rạc.

### Tóm tắt market context trong 3-4 dòng

> Các Tech Lead đang bị quá tải bởi việc review hàng tá PR mỗi ngày, dẫn đến review hời hợt và lọt bug. 
> Các tool cũ chỉ bắt được lỗi cú pháp chứ không hiểu logic nghiệp vụ. 
> Đây là lúc AI có thể giúp đọc hiểu logic toàn diện để giảm tải áp lực nhận thức cho lập trình viên.

---

## Bước 3 — Xác định `Job Executor`

`Job executor` là người **trực tiếp dùng một giải pháp để hoàn thành job**.

### Đừng nhầm với:

- người mua tiền nhưng không trực tiếp làm job
- người ảnh hưởng quyết định
- cả một công ty hay một phòng ban quá rộng

### Gợi ý viết cho đúng

- Sai hoặc quá rộng: `SME`, `doanh nghiệp`, `thị trường`
- Tốt hơn: `chủ shop online`, `nhân viên CSKH`, `recruiter`, `sales ops manager`

### Điền

- **Job executor của dự án này là:** Tech Lead / Senior Developer (Người chịu trách nhiệm review PR).
- **Vì sao tôi tin đây là người trực tiếp "thuê" giải pháp để làm job:**  
  > Vì họ là người tốn mồ hôi công sức nhất cho việc dò lỗi, và là người bị lôi ra chịu trách nhiệm đầu tiên nếu lọt bug nghiêm trọng lên production.

---

## Bước 4 — Viết `Core JTBD`

`Core JTBD` là công việc cốt lõi người dùng đang cố hoàn thành.

### Công thức gợi ý

```text
[verb] + [object] + [contextual clarifier]
```

### Ví dụ

- Chưa tốt: `trả lời inbox bằng AI`
- Tốt hơn: `giải quyết câu hỏi trước mua hàng nhanh và chính xác trong giờ cao điểm`

- Chưa tốt: `dùng AI để viết nội dung`
- Tốt hơn: `tạo bản nháp nội dung chiến dịch phù hợp với brand trong thời gian rất ngắn`

### 3 tiêu chí tự kiểm

- [ ] Nếu bỏ tool hiện tại đi, job này vẫn còn tồn tại
- [ ] Trong câu không có tên sản phẩm, AI, chatbot, app, màn hình
- [ ] Câu đang mô tả **điều user muốn hoàn thành**, không phải thứ product đang làm

### Bản nháp 1

**Core JTBD bản nháp:**  
> Dùng AI để tự động tìm bug và review code cho Tech Lead.

### Gạch bỏ từ solution nếu có

- Các từ solution tôi đang lỡ nhét vào câu: AI, tự động tìm bug, review code.

### Bản chốt

**Core JTBD cuối cùng:**  
> Đánh giá chất lượng và rủi ro của đoạn code mới thay đổi một cách nhanh chóng, chính xác trước khi đưa vào môi trường thực tế.

---

## Bước 5 — Viết 3 `Job Stories`

Nếu `core JTBD` là job ở mức cốt lõi, thì `job story` giúp bạn thấy
**job này xuất hiện trong hoàn cảnh nào**.

### Format

```text
When [trigger], I want to [motivation], so I can [outcome].
```

### Ví dụ

`When inbox đổ dồn vào buổi tối, tôi muốn có câu trả lời nhất quán ngay lập tức, so I can không mất đơn vì phản hồi chậm.`

### Bảng 3 job stories

| # | Trigger / When | Motivation / I want to | Outcome / so I can | Điều story này cho thấy |
|---|---|---|---|---|
| JS1 | Khi có một PR lớn với hàng trăm dòng thay đổi | Tôi muốn xác định ngay các điểm rủi ro bảo mật cốt lõi | So I can tập trung review sâu vào các file đó thay vì dò từng dòng mắt thường | Nhu cầu đánh giá mức độ nghiêm trọng (Triage) |
| JS2 | Khi tôi đang duyệt code của Junior Dev | Tôi muốn chỉ ra các điểm vi phạm best practices và convention | So I can giúp họ học hỏi mà không tốn công gõ comment giải thích dài dòng | Nhu cầu duy trì chuẩn mực code (Standard) |
| JS3 | Khi hệ thống sắp đến deadline release | Tôi muốn đảm bảo code mới không vô tình phá hỏng các luồng chức năng cũ | So I can yên tâm duyệt bài và không lo bị gọi dậy giữa đêm vì sự cố | Nhu cầu phân tích tác động chéo (Impact analysis) |

### Tự kiểm nhanh

- [ ] Mỗi story là một **tình huống thật**, không phải slogan chung chung
- [ ] 3 story không trùng hệt nhau
- [ ] Sau khi đọc 3 story, tôi hình dung được lúc nào product của mình đáng xuất hiện

---

## Bước 6 — Liệt kê `Current Alternatives`

Qua JTBD lens, đối thủ không chỉ là app cùng ngành.
Đối thủ là **bất kỳ thứ gì user đang "thuê" để làm job**:

- thao tác tay
- file Excel / Google Sheets
- intern / nhân viên
- agency
- ChatGPT / Claude / Gemini
- công cụ chuyên dụng khác
- hoặc thậm chí là **không làm gì cả**

### Bảng alternatives

| Alternative hiện tại | User đang thuê nó để làm gì? | Nó làm tốt gì? | Nó fail ở đâu? | Switching cost hiện tại cao hay thấp? |
|---|---|---|---|---|
| Đọc mắt trên GitHub UI | Đọc hiểu logic thay đổi | Hiểu sâu nghiệp vụ dự án | Chậm, mỏi mắt, lọt bug nếu mất tập trung | Cao (workflow bắt buộc bao năm nay) |
| Tool phân tích tĩnh (SonarQube) | Bắt lỗi cú pháp, code smell | Nhanh, tự động | Rập khuôn, sinh ra nhiều cảnh báo rác (false positive), không hiểu business logic | Thấp |
| ChatGPT (Copy/Paste) | Giải thích đoạn code khó hiểu | Phản hồi ngay, hướng dẫn chi tiết | Rất tốn công copy, rủi ro lộ mã nguồn công ty | Thấp |

### Kết luận nhanh

**Nếu project của tôi biến mất hôm nay, user nhiều khả năng sẽ quay về:**  
> Đọc code thủ công bằng mắt thường trên GitHub kết hợp với các công cụ CI/CD check lỗi cú pháp đơn thuần.

---

## Bước 7 — Điền `JTBD Lite Map`

Đây là bản rút gọn của `job map` trong playbook.

### Mục tiêu

Không phải để làm consultant workshop hoàn chỉnh.  
Mục tiêu là nhìn ra:

1. workflow hiện tại của user đi qua những bước nào
2. bước nào đang đau nhất
3. AI có nên chen vào đó không

### 8 bước tham chiếu từ playbook

1. `Define`
2. `Locate`
3. `Prepare`
4. `Confirm`
5. `Execute`
6. `Monitor`
7. `Modify`
8. `Conclude`

> Không nhất thiết bước nào cũng quan trọng như nhau trong dự án của bạn.  
> Nếu ít liên quan, ghi `N/A`, đừng để trống.

### Bảng JTBD Lite Map

| Step | Trong workflow này user đang cố làm gì? | Hôm nay họ đang dùng gì? | Friction / pain hiện tại | Mức đau |
|---|---|---|---|---|
| Define | Nhận thông báo có PR mới cần review | Email, Slack | Bị đứt mạch làm việc hiện tại (context switch) | Med |
| Locate | Mở PR, tìm hiểu bối cảnh (ticket Jira, mô tả) | GitHub PR description | Dev viết mô tả quá sơ sài, người review không hiểu code này làm gì | High |
| Prepare | Kéo code về máy (nếu cần), xem danh sách file diff | Git CLI, GitHub UI | Khó nắm được luồng ảnh hưởng nếu file thay đổi quá dài | Med |
| Confirm | Rà soát logic, tìm rủi ro tiềm ẩn / side-effect | Mắt thường, kinh nghiệm | Rất dễ sót lỗi logic ngầm nếu không tập trung 100% | High |
| Execute | Viết comment yêu cầu sửa đổi (Request Changes) | GitHub comment | Lười viết giải thích cặn kẽ cho dev khác hiểu | Med |
| Monitor | Đợi dev sửa rồi review vòng 2 | GitHub | Quên mất ngữ cảnh lần trước mình vừa comment gì | Low |
| Modify | Phê duyệt PR (Approve) | GitHub button | Vẫn lo âu bấm nhầm gây lỗi prod | Med |
| Conclude | PR được merge, đóng ticket | GitHub, Jira | Không | N/A |

### Chốt 2 bước đau nhất

**Bước đau nhất #1:** Locate (Tìm hiểu bối cảnh của một PR sơ sài).  
**Bước đau nhất #2:** Confirm (Đảm bảo code không có side-effect hoặc lỗi logic ẩn).

**Vì sao đây là nơi đáng chú ý nhất:**  
> Vì đây là 2 bước đòi hỏi nỗ lực nhận thức (cognitive load) cực cao.
> Người review phải bắt não bộ hoạt động hết công suất để tự ghép nối context và dự đoán rủi ro.

---

## Bước 8 — Chỉ ra `AI Leverage Point`

Sau khi map workflow, mới hỏi:
**AI nên vào đâu, với vai trò gì, và vì sao là ở đó?**

### Nhắc nhanh

- Đừng nhét AI vào chỉ vì "có AI thì nghe hay"
- Nếu pain lớn nhất không nằm ở chỗ AI giải tốt, hãy thành thật ghi ra
- Nếu current alternative đã đủ tốt, project cần xem lại

### Bảng leverage point

| Step | AI nên giúp bằng cách nào? | Vì sao AI hợp ở đây? | Rủi ro chính nếu dùng AI |
|---|---|---|---|
| Locate | Tự động đọc diff và sinh bản tóm tắt PR (Summary) mạch lạc, giải thích "What & Why" | AI cực kỳ giỏi tóm tắt thông tin code phức tạp thành ngôn ngữ tự nhiên (dễ hiểu) | Bịaa ra chức năng không có thật (Hallucination) |
| Confirm | Quét diff và chỉ ra rủi ro logic, bảo mật trực tiếp trên từng dòng code | Khả năng đối chiếu tức thì với hàng triệu mẫu mã nguồn và lỗi phổ biến | Đưa ra quá nhiều cảnh báo rác (False Positive) làm phiền người dùng |

### Kết luận nhanh

**AI leverage point quan trọng nhất của dự án tôi là:**  
> Bước Confirm: Tự động phân tích PR diff và "Draft" (nháp) sẵn các comment chỉ ra lỗi logic tiềm ẩn để Tech Lead duyệt.

**Vì sao không phải ở bước khác:**  
> Nếu chỉ dừng ở tóm tắt (Locate), user vẫn phải mỏi mắt tự dò lỗi. Can thiệp vào khâu Confirm mới thực sự cắt giảm 50% thời gian review.

---

## Bước 9 — Viết `Product Hypothesis`

Bây giờ mới đến lúc viết hypothesis.

### Công thức gợi ý

```text
Nếu chúng ta giúp [job executor] làm [job / sub-job] tốt hơn ở bước [x],
bằng cách [AI leverage],
thì họ sẽ chuyển từ [current alternative] sang [hướng giải pháp của nhóm],
vì [giá trị rõ nhất].
```

### Bản hypothesis của tôi

> Nếu chúng ta giúp `Tech Lead` làm `việc phân tích rủi ro của PR` tốt hơn ở bước `Confirm`,  
> bằng cách `dùng AI tự động quét file diff và đề xuất comment lỗi trực tiếp`,  
> thì họ sẽ chuyển từ `việc rà soát mắt thường 100%` sang `dùng AI assistant của dự án`,  
> vì `giúp họ tiết kiệm được một nửa thời gian review và giảm stress.`

### Tín hiệu sớm nếu hypothesis này đúng

1. User chủ yếu phê duyệt (approve) các comment do AI gợi ý thay vì xoá bỏ chúng.
2. Thời gian trung bình để duyệt và đóng một PR giảm đi rõ rệt.

---

## Bước 10 — Liệt kê `Assumptions to Validate`

Job story chưa có research vẫn chỉ là **giả thuyết tốt hơn**, chưa phải sự thật.

### 5 assumption thường đáng kiểm

- Tôi đã chọn đúng `job executor`
- Pain này thật sự đủ đau và xảy ra đủ thường xuyên
- User sẽ đổi khỏi alternative hiện tại nếu có giải pháp tốt hơn
- AI thực sự tạo giá trị ở step tôi chọn
- User đủ tin kết quả AI để đưa vào workflow thật

### Bảng assumptions

| Assumption | Vì sao assumption này rủi ro? | Tôi đang có bằng chứng gì? | Cần validate bằng cách nào tiếp theo? |
|---|---|---|---|
| A1 | Tech Lead là người quyết định mua tool | Có thể Engineering Manager mới là người mua (Buyer) | Phỏng đoán | Khảo sát quy trình mua sắm phần mềm ở các công ty IT |
| A2 | User dám cho AI truy cập mã nguồn công ty | Ngân hàng / Tổ chức tài chính sẽ cấm ngay lập tức | Feedback từ dự án tương tự | Đánh giá chuẩn bảo mật (SOC2, self-hosted LLM) |
| A3 | AI đủ sức hiểu logic sâu giữa các file với nhau | Các model thường bị giới hạn context window | Thử nghiệm với GPT-4 / Claude 3.5 | Chạy thử trên 50 PR lỗi thật xem AI có bắt đúng không |
| A4 | User đủ kiên nhẫn nếu AI báo lỗi sai | Nếu sinh ra quá nhiều cảnh báo rác, dev sẽ tắt tool | Quan sát behavior với SonarQube | Đo tỷ lệ Accept rate của AI comment trong Beta |
| A5 | | | | |

### Assumption nguy hiểm nhất nếu tôi đang sai

> Công ty dám cho phép AI bên thứ 3 truy cập vào kho mã nguồn (Bảo mật). Nếu điều này sai, sản phẩm sẽ chết ngay từ vòng đàm phán hợp đồng (compliance).

---

## Bước 11 — Share trong bàn (3')

### Mỗi người / mỗi nhóm chỉ nói 4 thứ

1. **Job executor của bạn là ai**
2. **Core JTBD của bạn là gì**
3. **Step đau nhất đang nằm ở đâu**
4. **AI leverage point + assumption rủi ro nhất là gì**

### Nếu chưa biết hỏi ngược gì, dùng 4 câu này

1. **"Câu JTBD này có đang lỡ nhét solution vào không?"**
2. **"Alternative hiện tại của user là gì, và tại sao họ chưa bỏ nó?"**
3. **"Pain mạnh nhất nằm ở bước nào trong workflow, có chắc AI giải tốt được không?"**
4. **"Assumption nào nếu sai thì cả hypothesis sẽ sập?"**

### Ghi nhanh sau khi nghe bàn phản biện

| Ý phản biện tôi nghe được | Nó chạm vào phần nào? | Tôi sẽ giữ / sửa gì? |
|---|---|---|
| Ngân hàng sẽ không bao giờ cho tool đẩy code lên cloud ngoài | Assumption về Security | Sẽ phải thiết kế phương án On-premise (chạy model nội bộ) ngay từ đầu |
| Tech Lead không phải là người trả tiền | Job Executor / Buyer | Giữ nguyên Executor là Tech Lead, nhưng ghi nhận thêm Manager là Buyer |
| AI hay sinh ra comment rác làm phiền Dev | AI Leverage point | Điều chỉnh tính năng: AI chỉ "Draft" (lưu nháp) để người review tự quyết định chứ không tự push comment |

---

## Bước 12 — Chốt version cuối sau thảo luận

### Sau khi nghe phản biện, tôi thay đổi gì?

- [x] Giữ nguyên `job executor`
- [ ] Sửa `job executor`
- [x] Giữ nguyên `core JTBD`
- [ ] Sửa `core JTBD`
- [ ] Giữ nguyên `AI leverage point`
- [x] Sửa `AI leverage point`
- [ ] Giữ nguyên `product hypothesis`
- [x] Sửa `product hypothesis`

### Vì sao tôi giữ / sửa?

> Nhận được phản biện rất hợp lý: AI chưa thể thay thế người duyệt 100% và rất dễ sinh rác. 
> Cần sửa lại Hypothesis và Leverage point để AI lùi lại một bước thành "người soạn nháp comment" (Copilot) thay vì "Tự động comment thay Dev" (Autopilot).

### Version cuối cùng tôi nộp

**Job executor:**  
> Tech Lead / Senior Developer (Người có trách nhiệm review). 

**Core JTBD:**  
> Đánh giá chất lượng và rủi ro của đoạn code mới một cách nhanh chóng và chuẩn xác trước khi release.

**2 bước đau nhất trong workflow:**  
> Locate (Mất nhiều công sức tìm hiểu bối cảnh PR) & Confirm (Vắt óc tìm các lỗi logic ngầm).

**AI leverage point chính:**  
> Tự động tạo bản Tóm tắt PR (Locate) và "Nháp" sẵn các comment rủi ro logic để người review quyết định có gửi hay không (Confirm).

**Product hypothesis:**  
> Nếu giúp Tech Lead ở khâu Confirm bằng cách quét rủi ro và nháp sẵn comment, họ sẽ dùng tool vì nó cắt giảm 50% effort đọc code thủ công nhưng vẫn giữ quyền kiểm soát cuối cùng.

**Assumption cần validate đầu tiên:**  
> Security Compliance: Các công ty tiềm năng có chấp nhận tích hợp mã nguồn của họ với LLM API hay bắt buộc phải chạy Local LLM?

---

## Checklist trước khi nộp

- [x] Tôi đã khoanh đúng 1 lát cắt cụ thể của dự án.
- [x] Tôi đã phân biệt được `job executor` với buyer / influencer.
- [x] `Core JTBD` của tôi không nhét solution vào câu.
- [x] Tôi đã viết đủ 3 `job stories`.
- [x] Tôi đã điền `JTBD lite map` và khoanh ra 2 bước đau nhất.
- [x] Tôi đã chỉ ra `AI leverage point` thay vì nhảy thẳng vào feature list.
- [x] Tôi đã ghi rõ `assumptions to validate`.
- [x] Tôi đã sửa version cuối sau khi share trong bàn.

---

## Nếu còn thời gian / làm về nhà

- Phỏng vấn nhanh 1 người dùng thật để kiểm xem `job story` nào là sát nhất.
- So sánh `current alternatives` với project của nhóm theo 3 tiêu chí: nhanh hơn, rẻ hơn, tin hơn.
- Tự hỏi lại một câu khó: **nếu không dùng AI, project này còn tạo giá trị không?**
- Nếu câu trả lời là "không", hãy xem lại liệu nhóm đang giải **job thật** hay chỉ đang tìm chỗ để nhét AI.
