---
artifact: 01 — Case Analysis
bai-tap: Lab 1 — Phân tích "tử huyệt" chiến lược
format: Cá nhân trước → share trong bàn → chốt verdict cuối
time: 20 phút trên lớp
nop-cuoi: Có — đây là file nộp cuối của Lab 1
---

# Lab 1 — Case Analysis / Phân tích "tử huyệt" chiến lược

**Case đã chọn:** Stack Overflow (mảng Public Q&A)  
**Người làm:** Nam  
**Bàn / nhóm bàn:** 
**Ngày:** 18/06/2026

> Đây là **file duy nhất** của Lab 1.  
> File này đồng thời đóng vai trò:
>
> - guide từng bước,
> - worksheet để điền trực tiếp,
> - và file nộp cuối cho người chấm.

Mục tiêu của bài này không phải kể lại "AI đã giết một công ty". Mục tiêu là chỉ ra, bằng bằng chứng thật:

1. **vì sao case đó bị tổn thương trước AI**
2. **điều gì đã thay đổi vĩnh viễn**
3. **và nếu rút một cảnh báo cho dự án của nhóm mình thì đó là gì**

Quy tắc xuyên suốt: **không có bằng chứng = không có nhận định.**

---

## Đầu ra bắt buộc

Người chấm cần thấy đủ 4 phần trong chính file này:

1. **3-5 bằng chứng chốt**
2. **4 nhận định bắt buộc**
3. **ghi chú sau khi share trong bàn**
4. **verdict cuối của cá nhân**

Nếu thiếu một trong bốn phần trên, bài sẽ bị xem là chưa hoàn chỉnh.

---

## Cách làm trong lớp (20 phút)

```text
2'  Chọn case
8'  Làm cá nhân: gom bằng chứng + viết 4 nhận định
7'  Share trong bàn: 90 giây / người + hỏi vặn lại
3'  Tự sửa verdict cá nhân sau thảo luận
```

---

## Bước 0 — Chọn case thật nhanh

Mặc định: **bạn tự chọn case của mình**.

### Một case phù hợp cần có 4 điều

- [ ] Có một **AI shock** hoặc mốc đổi cục diện đủ rõ
- [ ] Có thể tìm được ít nhất **3-5 bằng chứng công khai**
- [ ] Có tác động đủ nhìn thấy được ở user / doanh thu / pricing / traffic / cổ phiếu / usage / vị thế cạnh tranh
- [ ] Có thể trả lời câu hỏi: **"Điều gì đã thay đổi vĩnh viễn?"**

### Điền nhanh trước khi làm

- **Case / sản phẩm / công ty:** Stack Overflow (mảng diễn đàn hỏi đáp lập trình cộng đồng)
- **AI / platform / sản phẩm mới tạo áp lực:** ChatGPT & GitHub Copilot
- **Vì sao tôi chọn case này?**  
  > Đây là minh chứng rõ ràng cho việc nguồn sống cốt lõi (traffic và content mới) đang bị cắt đứt, dù họ từng sở hữu "Hiệu ứng mạng" khổng lồ.

### Nếu bí case, chọn 1 trong 6 case gợi ý này

| Case | Vì sao đáng phân tích | Một tín hiệu đáng chú ý |
|---|---|---|
| Chegg | entry point học tập đổi rất nhanh | 7,8M → 3,2M thuê bao |
| Stack Overflow | hiệu ứng mạng bị đảo chiều | câu hỏi mới giảm mạnh sau ChatGPT |
| Jasper | lớp vỏ dễ bị generic AI ép | định giá và tăng trưởng chậm lại sau ChatGPT |
| Tome | AI phổ thông "đủ tốt" làm phân khúc cũ yếu đi | nhiều đợt cắt giảm và pivot |
| Inflection / Pi | chatbot tiêu dùng bị ông lớn lấn át | đội ngũ chuyển sang Microsoft |
| Figma / Claude Design | rủi ro "đất thuê" khi platform bước xuống app layer | cổ phiếu Figma phản ứng tiêu cực khi Claude Design ra mắt |

> Nếu có case riêng rõ hơn, dùng case riêng.

---

## Bước 1 — Gom 3-5 bằng chứng chốt

Không cần chép lại mọi số. Chỉ giữ những bằng chứng đủ mạnh để đỡ toàn bộ lập luận của bạn.

### Tìm bằng chứng theo 4 cụm

1. **Case trước AI**
   Sản phẩm là gì, user là ai, họ trả tiền cho cái gì, case từng thắng nhờ gì.

2. **AI shock**
   Mốc Big Tech AI / platform AI / sản phẩm mới xuất hiện và đổi luật chơi.

3. **Tác động quan sát được**
   User, doanh thu, ARR, pricing, traffic, usage, cổ phiếu, sa thải, pivot.

4. **Cục diện mới của thị trường**
   Ai phản ứng tốt hơn, ai thay thế tốt hơn, entry point mới nằm ở đâu, phân khúc còn sống không.

### Ưu tiên nguồn thế nào?

| Mức ưu tiên | Loại nguồn | Ví dụ |
|---|---|---|
| 1 | Nguồn gốc | báo cáo tài chính, investor relations, pricing page, blog chính thức |
| 2 | Báo uy tín | Reuters, CNBC, Bloomberg, FT, TechCrunch |
| 3 | Dữ liệu công khai / tổng hợp | MacroTrends, Similarweb, Stack Overflow Survey, Sacra |

### Bảng bằng chứng chốt

| # | Bằng chứng / số liệu chốt | Vì sao số này quan trọng? | Nguồn |
|---|---|---|---|
| E1 | Traffic giảm khoảng 50% (từ >110 triệu lượt/tháng năm 2022 xuống ~55 triệu năm 2024) | Phản ánh trực tiếp việc người dùng bỏ đi do AI thay thế. | tms-outsource.com / Similarweb |
| E2 | Lượng câu hỏi mới tụt dốc thảm hại về mức của năm 2009 | Báo hiệu "cái chết" của hệ sinh thái nội dung do người dùng tạo. | Báo cáo cộng đồng SO |
| E3 | Sa thải đến 28% nhân sự vào tháng 10/2023 | Bằng chứng thực tế nhất cho sức ép doanh thu và hoảng loạn chiến lược. | Báo chí công nghệ |
| E4 | | | |
| E5 | | | |

### 3 phát hiện ban đầu

Trước khi viết nhận định, ghi nhanh 3 dòng:

1. **Case này từng thắng nhờ...**  
   > Kho tàng giải pháp và SEO Google, biến nó thành "cửa vào" bắt buộc của giới dev khi gặp lỗi.
2. **AI shock làm thay đổi...**  
   > "Entry point" (điểm bắt đầu). Điểm bắt đầu dời thẳng vào không gian làm việc (IDE) thay vì ra web tìm kiếm.
3. **Dấu hiệu mạnh nhất cho thấy luật chơi mới là...**  
   > Lượng traffic giảm 50% và việc công ty phải sa thải 28% nhân sự.

---

## Bước 2 — Viết 4 nhận định bắt buộc

### Nhận định 1 — Trước AI, case này thắng nhờ giả định gì?

Gợi ý:

- Người dùng thuê sản phẩm này để làm gì?
- Giá trị lõi trước AI là gì?
- Họ thắng nhờ workflow, switching cost, brand, distribution, data hay một giả định hành vi nào?
- Job-to-be-done (công việc người dùng "thuê" sản phẩm làm hộ) là gì?

**Trả lời của tôi:**  
> Trước đây, quy trình chuẩn là: gặp lỗi -> copy lỗi -> paste lên Google -> vào Stack Overflow tìm câu trả lời có nhiều upvote -> tự sửa. 
> Họ thắng nhờ kho tàng giải pháp khổng lồ và SEO Google mạnh, biến diễn đàn thành "cửa vào" bắt buộc.

**Bằng chứng đỡ nhận định này:** E1

---

### Nhận định 2 — Kỳ vọng người dùng và luật chơi cạnh tranh đã đổi ở đâu?

#### Nhắc nhanh 7 Dịch chuyển Kỳ vọng

1. Làm xong giúp tôi
2. May đo cho tôi
3. Tự lo việc lặt vặt
4. Trả theo kết quả
5. Phản hồi ngay
6. Giao diện tự thay đổi
7. Thấu hiểu ngữ cảnh

#### Nhắc nhanh 5 Competitive Dynamics

- switching costs giảm
- data advantages tăng
- platform risk
- build-copy cycles tăng tốc
- GTM + distribution quan trọng hơn

**Shift kỳ vọng quan trọng nhất:** 1. Làm xong giúp tôi & 5. Phản hồi ngay  
**Competitive dynamic quan trọng nhất:** GTM + distribution quan trọng hơn (Platform dời xuống IDE)

**Trả lời của tôi:**  
> Lập trình viên có thể hỏi thẳng AI ngay tại dòng code đang lỗi, AI thấu hiểu toàn bộ ngữ cảnh và viết lại code luôn cho họ.
> User shift sang kỳ vọng "Làm xong giúp tôi" thay vì "Chỉ tôi cách làm".

**Bằng chứng đỡ nhận định này:** E1, E2

---

### Nhận định 3 — Giả định nào không còn đúng nữa? Điều gì đã thay đổi vĩnh viễn?

Gợi ý:

- Switching cost cũ có từng giữ user ở lại không? Vì sao giờ không còn đủ?
- Entry point cũ của sản phẩm có còn tồn tại không, hay người dùng đã chuyển sang một điểm bắt đầu mới?
- Workflow cũ có còn được chấp nhận không, hay chuẩn mới là "làm xong giúp tôi / ngay trong nơi tôi đang làm việc"?
- "Thay đổi vĩnh viễn" không phải là giá cổ phiếu giảm; nó là **chuẩn mới trong đầu người dùng** hoặc **luật chơi mới của thị trường**.
- Phân khúc này còn tồn tại không? Nếu còn, nó đang được phục vụ theo cách khác ra sao?

**Điều đã thay đổi vĩnh viễn theo tôi là:**  
> "Entry point" (điểm bắt đầu) và quy trình làm việc (workflow) của lập trình viên đã dời thẳng vào không gian làm việc (IDE). 
> Stack Overflow mất lợi thế vì kho tàng giải pháp và SEO Google của họ không còn là "cửa vào" bắt buộc nữa.

**Bằng chứng đỡ nhận định này:** E1, E2

---

### Nhận định 4 — Case này còn cứu được không? Nếu có, phải đổi bằng cách nào?

Gợi ý:

- Nếu cứu được: họ phải đổi ở moat nào, workflow nào, distribution nào?
- Nếu không cứu được: vì sao đã quá muộn?
- So với một đối thủ phản ứng tốt hơn, họ chậm ở đâu?

**Verdict ban đầu của tôi:** Có nhưng phải đổi rất mạnh

**Trả lời của tôi:**  
> Mô hình hỏi đáp truyền thống phụ thuộc vào web traffic và quảng cáo của Stack Overflow gần như đã sụp đổ.
> Tuy nhiên, case này vẫn có thể "sống" nếu họ pivot thành công bằng cách đóng vai trò là nguồn cấp dữ liệu chất lượng cao (Data Licensing) để huấn luyện LLM, hoặc đẩy mạnh OverflowAI (nhúng thẳng vào IDE).

**Bằng chứng đỡ nhận định này:** E3

---

## Tóm tắt cá nhân trước khi share trong bàn

Viết đúng 3 câu:

1. `Case này yếu đi vì...`
2. `Điều thay đổi vĩnh viễn là...`
3. `Verdict của tôi là...`

**Bản tóm tắt 3 câu của tôi:**  
1. `Case này yếu đi vì mô hình phụ thuộc web traffic bị sụp đổ, lượng câu hỏi mới tụt thảm hại.`  
2. `Điều thay đổi vĩnh viễn là "Entry point" và workflow dời thẳng vào IDE, user chuyển sang kỳ vọng "Làm xong giúp tôi".`  
3. `Verdict của tôi là SO phải pivot thành nguồn cấp dữ liệu (Data Licensing) hoặc làm OverflowAI thì mới sống được.`

---

## Bước 3 — Share trong bàn (7')

### Mỗi người chỉ nói 4 thứ trong 90 giây

1. **Case bạn chọn là gì**
2. **Bằng chứng mạnh nhất bạn có là gì**
3. **Điều gì đã thay đổi vĩnh viễn**
4. **Verdict của bạn**

### Nếu chưa biết hỏi ngược gì, dùng 4 câu này

1. **"Bằng chứng mạnh nhất cho nhận định đó là gì?"**
2. **"Điều gì ở đây là triệu chứng, còn điều gì là thay đổi vĩnh viễn?"**
3. **"Nếu switching cost từng cao, vì sao người dùng vẫn rời đi?"**
4. **"Platform mới hoặc đối thủ mới đã chiếm entry point ở đâu?"**

### Ghi nhanh khi nghe các bạn cùng bàn

| Người | Case | Bằng chứng mạnh nhất họ nêu | Điều họ cho là "thay đổi vĩnh viễn" | Verdict của họ |
|---|---|---|---|---|
| Đỗ Tuấn Đạt | Shutterstock | Lượt tải giảm 11.7%, subscriber giảm 14.7% (Q3/2024), doanh thu Content giảm 7% | Entry point chuyển từ "tìm ảnh có sẵn" (search) sang "tạo ảnh theo yêu cầu" (generate) | Còn cứu được nhưng phải tích hợp tạo/chỉnh sửa AI và bán data |
| Hoàng Hiếu Trung | Chegg | Subscriber giảm từ 7.8M xuống 3.2M, CEO thừa nhận ChatGPT chặn đứng tăng trưởng | Entry point chuyển từ Search Google -> Chegg sang hỏi thẳng AI Chatbot | Phải pivot sang học tập cá nhân hóa, mô hình trả phí giải bài tập cũ đã chết |
| Bạn 3 | | | | |
| Bạn 4 | | | | |

### Sau khi cả bàn share xong, chốt 3 ý chung

**1. Bàn tôi thấy case nào có bằng chứng mạnh nhất? Vì sao?**  
> Case Stack Overflow. Vì có bằng chứng cực mạnh về traffic giảm 50% và sa thải 28% nhân sự.

**2. Có pattern nào lặp lại giữa nhiều case không?**  
Ví dụ: switching costs giảm, platform bước xuống app layer, user chuyển sang "làm xong giúp tôi", moat cũ quá mỏng…  
> Sự chuyển dịch sang "làm xong giúp tôi" và platform (AI) bước thẳng vào app layer (IDE) để chiếm lấy entry point.

**3. Một cảnh báo cho chính dự án của nhóm tôi là gì?**  
> Dù bạn có "Hiệu ứng mạng" lớn đến đâu, AI vẫn có thể cướp đi điểm chạm (entry point) của bạn nếu bạn không đón đầu workflow.

---

## Bước 4 — Chốt lại verdict cá nhân sau thảo luận (3')

### Sau khi nghe bàn phản biện, verdict của tôi:

- [x] Giữ nguyên
- [ ] Đổi nhẹ
- [ ] Đổi mạnh

### Vì sao tôi giữ / đổi verdict?

> Tôi giữ nguyên verdict vì mô hình cũ đã chết, họ bắt buộc phải pivot sang Data Licensing và OverflowAI như nhận định ban đầu.

### Verdict cuối cùng của tôi (phiên bản nộp)

**Case này tổn thương trước AI vì:**  
> Nguồn sống cốt lõi (traffic và content mới) bị cắt đứt. Quy trình truyền thống "copy lỗi -> paste Google -> đọc SO" đã bị AI thay thế hoàn toàn.

**Điều thay đổi vĩnh viễn là:**  
> "Entry point" của lập trình viên đã dời thẳng vào IDE, AI thấu hiểu ngữ cảnh và "Làm xong giúp tôi". SEO và kho tàng giải pháp trên web không còn là cửa vào bắt buộc.

**Nếu phải rút 1 bài học cho dự án của nhóm mình, tôi rút ra:**  
> Đây là case kinh điển về việc dù bạn có "Hiệu ứng mạng" (Network Effect) lớn đến đâu, AI vẫn có thể cướp đi điểm chạm (entry point) của bạn.

---

## Checklist trước khi nộp

- [x] Tôi đã chọn ít nhất 3 bằng chứng chốt có nguồn.
- [x] Mỗi nhận định đều chỉ vào ít nhất 1 bằng chứng.
- [x] Tôi đã ghi lại phần share trong bàn.
- [x] Tôi đã viết verdict cuối sau thảo luận.

---

## Nếu còn thời gian / làm về nhà

- Bổ sung thêm một case "đối thủ phản ứng tốt hơn" để so.
- Thêm một đoạn ngắn: **nếu tôi là PM của case này trong 6 tháng đầu sau AI shock, tôi sẽ làm gì đầu tiên?**
- Kiểm lại xem case này yếu vì expectation shift, competitive dynamics, hay cả hai cùng lúc.
