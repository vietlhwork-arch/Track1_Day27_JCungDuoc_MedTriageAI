# Bài làm cá nhân — Lê Hoàng Việt · `2A202601543`

**Nhóm JCungDuoc** · Dự án **MedTriage AI** · Day 27 · 29/08/2026
**Vai trò dự án:** AI Product Owner / Founder — **Trưởng nhóm, người tổng hợp repository**

> File này chứa **phần tôi tự làm trước khi thảo luận** ở Phase 1.1, Phase 2.3 và Phase 4.1.
> Nó được giữ nguyên như lúc viết, kể cả những chỗ sau đó nhóm sửa hoặc bác bỏ — vì giá trị của bước
> cá nhân nằm ở chỗ nó cho thấy **mỗi người thiếu gì**, không phải ở chỗ ai đúng.

---

## Phase 1.1 — Stakeholder tôi tự liệt kê (5 phút, chưa thảo luận)

Tôi liệt kê được **8 stakeholder**. Góc nhìn của tôi nghiêng rõ về **thương mại và học thuật** — đúng
với việc tôi là người đang giữ mô hình kinh tế và các quan hệ bên ngoài.

| # | Stakeholder tôi ghi | Influence | Interest | Stance tôi đoán | Vào bản đồ chung? |
|---|---|---|---|---|---|
| 1 | Giảng viên / mentor Track 1 đang review dự án từ Day 22 | Cao | Cao | Ủng hộ | ✔ **S5** |
| 2 | Cố vấn tài chính ngoài công ty (đã nhận dự cổng gác ngày 90) | Trung bình–Cao | Cao | Ủng hộ | ✔ **S6** |
| 3 | Trưởng khoa Cấp cứu bệnh viện pilot A | Cao | Cao | Trung lập | ✔ **S1** |
| 4 | Ban Giám đốc + Phòng Tài chính–Kế toán bệnh viện A (người ký hợp đồng) | Cao | Thấp | Chưa ủng hộ | ✔ **S2** |
| 5 | Quỹ ươm tạo / nhà đầu tư thiên thần | Thấp | Thấp | Trung lập | ✔ **S10** |
| 6 | Trưởng phòng CNTT bệnh viện A | Cao | Thấp | Chưa rõ | ✔ **S4** *(tôi ghi mờ, Hưng làm rõ)* |
| 7 | Bệnh nhân & người nhà ở hàng chờ cấp cứu | Thấp | Cao | Trung lập | ✔ **S8** |
| 8 | Bảo hiểm y tế / đơn vị chi trả | Thấp | Thấp | Chưa rõ | ✘ **loại** |

**Tôi loại #8 khi vào phần Team.** Ở mô hình hiện tại bệnh viện là người trả tiền trực tiếp (phí nền + phí
theo ca), không đi qua đơn vị chi trả. Giữ lại chỉ để bản đồ trông đầy đủ là đúng thứ đề bài cảnh báo.

### Thứ tôi thiếu, và chỉ lộ ra vì làm cá nhân trước

**Danh sách của tôi không có S3 — điều dưỡng tiếp nhận.** Tôi liệt kê được người *ký hợp đồng*, người *duyệt
ngân sách*, người *đầu tư*, nhưng bỏ sót đúng **người sẽ phải bấm vào sản phẩm mỗi ca trực**. Linh là người
bổ sung S3. Đây là lỗ hổng nghiêm trọng nhất của tôi hôm nay: tôi đang nhìn dự án qua bảng giá và cổng gác,
nên vô thức xếp người dùng thật ra ngoài rìa. Nó khớp đúng với việc tôi tự chấm "Chất lượng AI" **4/5**
trong khi Linh chấm **2/5** (xem Phase 4 bên dưới).

---

## Phase 2.3 — Bản pitch tôi tự viết lại (5 phút)

**Gửi:** S1 — Trưởng khoa Cấp cứu, Bệnh viện A

> **Kết luận.** Tôi đề nghị khoa cho MedTriage AI chạy **shadow mode 2 tuần, ca trực ngày 7h–15h, mục tiêu
> 200 ca**. AI không hiển thị bậc ưu tiên cho bất kỳ ai; nó chỉ sinh phiếu SBAR song song để khoa đối chiếu
> sau ca. Không đổi quy trình tiếp nhận, không nối HIS, không cần chữ ký của phòng tài chính.
>
> **Lý do.** (1) Nút thắt của khoa nằm ở thời gian tiếp nhận, không nằm ở quyết định lâm sàng — chúng tôi chỉ
> nhận đúng phần trước quyết định. (2) Điều dưỡng vẫn là người ký và người quyết định, ranh giới này chúng tôi
> chốt từ đầu và không đổi. (3) Sau 2 tuần khoa có số đo của chính khoa mình, thứ hiện chưa ai có.
>
> **Bằng chứng.** Mô hình kinh tế đã dựng đủ và kiểm chứng ngược được bằng script — 22/22 phép kiểm tra khớp:
> giá 6.000.000 ₫/tháng + 13.000 ₫/ca, chi phí AI 2.307 ₫/ca, gross margin 71,8%, breakeven containment 55,1%.
> Luật an toàn viết trước khi chạy: under-triage vượt 3,0% trong một tuần thì tắt đề xuất bậc ưu tiên trong 24h.
> **Điều tôi chưa có:** containment 78% là ước tính dựng từ dưới lên, chưa từng đo trên ca thật.
>
> **Small ask.** Xin 45 phút với một điều dưỡng trưởng ca để chốt luồng, và chữ ký đồng ý cho 2 tuần shadow
> bắt đầu 15/09/2026.

**Nhóm giữ lại từ bản của tôi:** câu **Kết luận** (vì nó nêu luôn small ask ngay trong câu đầu) và toàn bộ
**phần số liệu** của Bằng chứng.
**Nhóm sửa của tôi:** bản gốc tôi viết xin thêm *"quyền truy cập HIS ở chế độ chỉ đọc"*. Hưng chỉ ra rằng
xin HIS là kéo S4 vào từ tuần đầu và biến một small ask thành một dự án. **Đã cắt.** Đây là góp ý làm bản
cuối tốt lên rõ nhất.

---

## Phase 4.1 — Điểm Team Health tôi tự chấm (chưa nhìn điểm ai)

| Khía cạnh | Điểm tôi chấm | Tôi đang nhìn vào cái gì khi chấm |
|---|:---:|---|
| **Chất lượng AI** | **4** | Tôi chấm chất lượng **bản thiết kế**: mô hình kinh tế kiểm chứng ngược 22/22, dashboard 8 đèn đủ ngưỡng, 4 luật dừng, 3 cổng gác có kill criteria. Theo tiêu chuẩn tài liệu thì đây là 4. |
| **Tiến độ** | **4** | Day 22 → Day 26 không buổi nào trượt hạn, artefact nào cũng nộp đủ. |
| **Tinh thần team** | **4** | Ba người nói thẳng được vấn đề, không ai giấu phần mình chưa làm. |
| **Tốc độ ra sản phẩm** | **2** | Không có một ca thật nào. Mọi thay đổi 5 ngày qua chỉ đi từ tài liệu này sang tài liệu khác. |

### Sau khi so điểm — tôi đã sai ở đâu

Linh chấm **Chất lượng AI = 2**, chênh tôi **2 điểm**. Truy ra thì **tôi đang chấm chất lượng tài liệu, Linh
đang chấm chất lượng đầu ra lâm sàng**. Linh đúng ở chỗ quan trọng hơn: bộ eval không tồn tại, under-triage
chưa đo, chưa ca thật nào — theo tiêu chuẩn "sản phẩm" thì đây là 2, không phải 4.

**Điều tôi rút ra và ghi vào Trang 4 của bài nộp:** *đội đang nhầm "tài liệu chặt" với "sản phẩm tốt".*
Chính tôi là người tạo ra sự nhầm lẫn đó, vì tôi là người sản xuất phần lớn tài liệu. Nó khớp đúng với lời
tự phê tôi đã viết ở Day 26 — *"dashboard của một sản phẩm chưa chạy ca thật nào"* — nhưng hôm đó tôi ghi nó
như một ghi chú trung thực, còn hôm nay nó trở thành **vấn đề ưu tiên số 1 của cả nhóm**.

---

## Phần tôi chịu trách nhiệm trong bài nộp

- **Trang 1 — Stakeholder Map & Strategy:** toàn bộ, gồm 4 chiến lược và phần giải thích vì sao không chọn S2/S4.
- **Trang 2 — Pitch & RACI:** toàn bộ Pitch, phản biện, và cấu trúc RACI.
- **Chữ A trong RACI:** **T1** (chốt phạm vi shadow pilot & thuyết phục BV A) và **T6** (quyết định GO/FIX tại cổng gác ngày 30).
- **Growth Plan:** owner của **G-1** — gửi đề nghị shadow cho Trưởng khoa Cấp cứu, hạn gửi **03/09**, chốt ngày
  bắt đầu **12/09/2026**. Nếu bị từ chối, phải có văn bản lý do **và** tên bệnh viện thứ hai đã gửi.
- **Trách nhiệm trưởng nhóm:** tạo repository từ đầu Lab, giữ 4 trang nhất quán, export PDF, kiểm số trang,
  và **gửi link repo** để nộp bài.
