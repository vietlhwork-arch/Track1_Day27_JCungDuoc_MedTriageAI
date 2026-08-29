# Bài làm cá nhân — Hồ Phạm Đức Linh · `2A202601533`

**Nhóm JCungDuoc** · Dự án **MedTriage AI** · Day 27 · 29/08/2026
**Vai trò dự án:** Clinical Safety & Evals Lead — **chủ trì Phase 4 (Team Health & Growth Plan)**

> File này chứa **phần tôi tự làm trước khi thảo luận** ở Phase 1.1, Phase 2.3 và Phase 4.1.

---

## Phase 1.1 — Stakeholder tôi tự liệt kê (5 phút, chưa thảo luận)

Tôi liệt kê được **7 stakeholder**. Góc nhìn của tôi nghiêng về **phía lâm sàng và phía người bị ảnh hưởng** —
đúng với phần việc tôi đã làm ở Day 22 (harm map cho copilot chẩn đoán, 10 dòng đủ 7 failure layer).

| # | Stakeholder tôi ghi | Influence | Interest | Stance tôi đoán | Vào bản đồ chung? |
|---|---|---|---|---|---|
| 1 | **Điều dưỡng tiếp nhận (triage nurse)** — người ký phiếu SBAR | Thấp trên giấy / **Cao trên thực địa** | Cao | **Chưa ủng hộ** | ✔ **S3** — *tôi là người duy nhất ghi ra người này* |
| 2 | Trưởng khoa Cấp cứu bệnh viện A | Cao | Cao | Trung lập | ✔ **S1** |
| 3 | Bệnh nhân & người nhà đang chờ ở khoa cấp cứu | Thấp | Cao | Trung lập | ✔ **S8** |
| 4 | **Hội đồng Quản lý chất lượng / đạo đức bệnh viện** | Cao | Trung bình | Trung lập | ✔ **S9** — *tôi là người duy nhất ghi ra* |
| 5 | Bác sĩ trực cấp cứu nhận bàn giao SBAR | Trung bình | Cao | Trung lập | ✘ **gộp vào S1** |
| 6 | Giảng viên / mentor Track 1 | Cao | Cao | Ủng hộ | ✔ **S5** |
| 7 | Sở Y tế / cơ quan quản lý hành nghề | Cao | Thấp | Trung lập | ✘ **loại ở giai đoạn này** |

**Tôi loại #7 khi vào phần Team**, dù tiếc: ở phạm vi shadow mode, sản phẩm chưa phải thiết bị y tế và chưa
tác động lên quyết định lâm sàng, nên cơ quan quản lý chưa phải stakeholder có ảnh hưởng **trong 30 ngày tới**.
Nhóm ghi lại để mở lại **trước cổng ngày 60**, khi bắt đầu bàn tới hợp đồng thật.
**Tôi gộp #5 vào S1** vì bác sĩ trực và trưởng khoa cùng chung mối lo và cùng chung một cửa quyết định.

### Thứ tôi thiếu

**Danh sách của tôi không có S4 — trưởng phòng CNTT / quản trị HIS**, và cũng không có ai thuộc phía tài chính.
Tôi nhìn thấy toàn bộ đường đi của người bệnh nhưng không nhìn thấy **đường đi của dữ liệu và đường đi của tiền**.
Hưng bổ sung S4 và S7, Việt bổ sung S2 và S6. Nếu chỉ có bản đồ của tôi, nhóm sẽ đi vào bệnh viện mà không biết
ai giữ cửa VPC.

---

## Phase 2.2 — Phản biện tôi đề xuất (đây là phần tôi chủ trì)

Tôi đề xuất phản biện được đưa vào bài nộp, vì đây là câu **chắc chắn sẽ được hỏi** và cũng là câu nhóm
**không có số đo nào để bác lại**:

> **"AI chưa đủ đáng tin để đụng vào bệnh nhân cấp cứu. Nếu nó bỏ sót một ca nặng thì ai chịu trách nhiệm?"**

Tôi viết 3 trong 5 ý trả lời của bài nộp:

1. **Trong 2 tuần shadow, không tồn tại đường nào để AI gây under-triage** — đầu ra không tới người ra quyết định.
   Rủi ro cần bàn là rủi ro *sau* shadow, và nhóm đề nghị **đo nó trước rồi mới bàn**.
2. **Trách nhiệm pháp lý không đổi:** phiếu SBAR chỉ có giá trị khi điều dưỡng ký. Đây là ràng buộc nhóm tự đặt
   từ Day 22, cùng với kết luận `conditional-go` và **5 release blocker** chưa gỡ.
3. **Có luật dừng viết sẵn, không phải viết sau khi có sự cố:** R-03 (under-triage > 3,0% trong 1 tuần → tắt
   đề xuất bậc ưu tiên trong 24h) và R-02 (containment < 55,1% ba tuần liên tiếp → dừng toàn bộ bán hàng 30 ngày).

**Điều tôi kiên quyết đòi đưa vào Bằng chứng của Pitch:** phần **"Điều nhóm CHƯA có"**. Bản nháp đầu chỉ liệt kê
các con số đẹp. Một pitch y tế chỉ nói phần mạnh sẽ mất uy tín ngay lần đầu bị hỏi ngược, và tệ hơn là nó vi phạm
đúng luật số 3 của Lab: *không được hứa vượt quá bằng chứng hiện có*.

## Phase 2.3 — Bản pitch tôi tự viết lại (5 phút)

> **Kết luận.** Đề nghị khoa cho chạy **shadow mode 2 tuần**: AI làm phiếu SBAR song song, **không ai nhìn thấy
> đề xuất của AI**, để cuối 2 tuần khoa có số đo về việc AI thu thập đủ hay thiếu thông tin gì.
>
> **Lý do.** (1) Rủi ro lâm sàng của giai đoạn này **bằng 0 theo thiết kế**, không phải theo lời hứa — đầu ra
> không đi tới người ra quyết định. (2) Người quyết định vẫn là điều dưỡng và bác sĩ của khoa, không đổi một
> dòng quy trình. (3) Thứ khoa nhận được là dữ liệu về chính khoa mình.
>
> **Bằng chứng.** Nhóm có luật dừng viết trước khi chạy (under-triage > 3,0% → tắt đề xuất trong 24h) và một
> cổng gác ngày 30 cố ý không gắn doanh thu. **Nhóm chưa có:** bất kỳ ca thật nào, và containment 78% mới là
> ước tính chứ chưa phải số đo.
>
> **Small ask.** Xin một buổi 45 phút với điều dưỡng trưởng ca, và cho tôi được ngồi quan sát 2 ca trực để
> hiểu đúng luồng tiếp nhận trước khi bàn tiếp.

**Nhóm giữ lại từ bản của tôi:** câu **"rủi ro lâm sàng bằng 0 theo thiết kế, chứ không bằng lời hứa"** —
hai bản kia viết "rủi ro thấp", mà "thấp" thì không kiểm được. Và toàn bộ **phần "Điều nhóm CHƯA có"**.
**Ý của tôi không được đưa vào:** xin ngồi quan sát 2 ca trực. Việt lập luận rằng small ask phải là **một** việc
dễ gật đầu; xin thêm quyền quan sát làm lời đề nghị nặng lên. Tôi đồng ý — nhưng nhóm ghi lại để xin ngay sau
khi có chữ ký đầu tiên.

---

## Phase 4.1 — Điểm Team Health tôi tự chấm (chưa nhìn điểm ai)

| Khía cạnh | Điểm tôi chấm | Tôi đang nhìn vào cái gì khi chấm |
|---|:---:|---|
| **Chất lượng AI** | **2** | Tôi chấm chất lượng **đầu ra lâm sàng**: không có bộ eval nào, under-triage chưa đo, chưa một ca thật nào chạy. Với sản phẩm chạm tới bệnh nhân cấp cứu, chưa đo được nghĩa là chưa biết — điểm 2 là đã rộng lượng. |
| **Tiến độ** | **3** | Bài nộp thì đúng hạn, nhưng **milestone của sản phẩm** thì không: kế hoạch có pilot từ Day 25 và đến nay vẫn chưa bắt đầu. |
| **Tinh thần team** | **4** | Nói thẳng được vấn đề, không ai bảo vệ phần mình bằng mọi giá. Đây là điểm mạnh thật của nhóm. |
| **Tốc độ ra sản phẩm** | **2** | Đo bằng "bao lâu để một thay đổi tới tay người dùng thật" thì hiện nay là **vô hạn**. |

### Sau khi so điểm

Việt chấm Chất lượng AI **4**, tôi chấm **2** — chênh **2 điểm**, lớn nhất bảng. Không ai chấm sai: **chúng tôi
chấm hai thứ khác nhau.** Việt chấm chất lượng bản thiết kế, tôi chấm chất lượng đầu ra. Chênh lệch này chính là
thứ tôi đề nghị đưa thành **phát hiện chính của Phase 4**, vì nếu để nguyên thì nửa năm nữa nhóm vẫn sẽ tin là
mình đang làm tốt trong khi chưa có gì chạm tới bệnh nhân.

Tôi cũng đề nghị **chọn chính role của tôi** cho phần Competency thay vì chọn role người khác: tôi đang **gần L2 —
AI Practitioner** (đã dựng được harm map 10 dòng, 8 gap, 5 release blocker ở Day 22, **nhưng chưa từng chạy một
eval có số**), và năng lực còn thiếu của tôi — **Evals / quality evaluation** — đúng là năng lực đang chặn cả nhóm.

---

## Phần tôi chịu trách nhiệm trong bài nộp

- **Trang 4 — Team Health & Growth Plan:** toàn bộ, gồm phần phân tích chênh lệch điểm, vấn đề ưu tiên và
  khung competency L1/L2/L3.
- **Trang 1:** stance thực tế của **S1** và **S3** (hai chỗ lệch nhãn quadrant), và chiến lược cho S3.
- **Trang 2:** phản biện chính và 3/5 ý trả lời; phần "Điều nhóm CHƯA có" trong Bằng chứng.
- **Trang 3:** capability gap **G-1** (chuyên môn lâm sàng → **Partner**) và **G-3** (evals → **không Outsource**,
  chỉ Partner cho vòng thẩm định độc lập, phần lõi nâng nội bộ).
- **Chữ A trong RACI:** **T3** (chuẩn bị dữ liệu — 30 golden cases + bộ nhãn 420 ca) và **T4** (kiểm thử an toàn —
  đo under-triage, chạy eval mỗi release). Tôi cũng là người **có quyền bấm luật dừng R-03**.
- **Growth Plan:** owner của **G-2** — xây 30 golden cases có nhãn do điều dưỡng trưởng BV A ký nhận và dựng
  `make eval`, hạn **19/09/2026**. Dấu hiệu hoàn thành: chạy được trên máy cả ba người, và **≥25/30 ca có nhãn
  do người hành nghề y ký nhận**. Ở điểm kiểm ngày 14, nếu chưa đạt ≥10/30 thì **cắt xuống 20 ca** chứ tuyệt đối
  không tự gán nhãn thay người hành nghề cho đủ số.
