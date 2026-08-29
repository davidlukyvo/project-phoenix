# Editorial Voice — sangvo.me

## Mục tiêu

Website phải tạo cảm giác đây là những ghi chép của một người làm Infrastructure lâu năm: đã trải qua project thật, cutover thật, sự cố thật, rollback thật và vận hành thật.

Nội dung không cố làm mọi thứ nghe “vĩ mô”. Độ senior nên tự hiện ra qua bối cảnh, quyết định kỹ thuật, trade-off, cách kiểm chứng và bài học vận hành — không qua khẩu hiệu.

## Giọng viết

- Viết như đang kể lại một tình huống hoặc một bài học nghề nghiệp cho một engineer khác.
- Ưu tiên câu tự nhiên, rõ và cụ thể.
- Có thể dùng thuật ngữ tiếng Anh khi đó là cách dân Infra thực sự nói: cutover, rollback, failover, UAT, service validation, dependency, routing, HA, restore...
- Khi có thể nói bằng một câu đơn giản thì không dùng ba lớp thuật ngữ để làm câu nghe “enterprise” hơn.
- Không tự khen mình. Không nói “world-class”, “transformational”, “best-in-class”, “strategic leader” hoặc các cách diễn đạt tương tự.
- Không biến mỗi project thành một “transformation journey”. Gọi đúng bản chất: migration, thay thiết bị, chuẩn hóa access, dựng monitoring, kiểm tra restore, xử lý dependency...

## Cách chứng minh kinh nghiệm

Ưu tiên chi tiết có giá trị vận hành:

- Điều gì có thể hỏng?
- Team kiểm tra bằng cách nào?
- Device healthy có đồng nghĩa service healthy không?
- Trigger rollback là gì?
- Sau go-live còn phải quan sát gì?
- Một dashboard/HA/backup/tunnel “xanh” thực sự chứng minh được điều gì, và chưa chứng minh được điều gì?

Một chi tiết thực tế như GlobalProtect Pre-logon, OSPF convergence, restore validation hay một rollback trigger có sức nặng hơn một đoạn tự mô tả “engineering excellence”.

## Từ/cụm từ cần dùng có chừng mực

Các từ sau không bị cấm, nhưng chỉ dùng khi thật sự cần và có nội dung cụ thể phía sau:

- modernization
- transformation
- governance
- resilience
- operational readiness
- platform thinking
- architecture
- engineering
- capability
- business outcome

Nếu bỏ từ đó mà câu vẫn giữ nguyên ý, thường nên bỏ.

## Tiêu đề

Ưu tiên tiêu đề giống một câu hỏi hoặc một nhận xét rút ra từ thực tế:

- `Migration không bắt đầu ở Cutover`
- `Tunnel UP chưa có nghĩa là hệ thống đã thông`
- `HA xanh vẫn chưa đủ để Cutover thành công`
- `Hệ thống vẫn chạy tốt, tại sao vẫn phải thay?`

Tránh tiêu đề kiểu brochure/corporate nếu có thể diễn đạt gần gũi hơn.

## Mở bài

Nên đi vào bối cảnh thật nhanh. Tốt nhất trong 1–3 đoạn đầu người đọc hiểu được:

1. chuyện gì đang xảy ra,
2. vì sao nó đáng nói,
3. bài học hoặc câu hỏi chính của bài.

Không cần mở bằng tuyên ngôn lớn về ngành IT hay “kỷ nguyên chuyển đổi số”.

## Thân bài

- Kể theo diễn tiến của vấn đề hoặc quyết định.
- Tách rõ device validation và service validation khi phù hợp.
- Đưa command/checklist/sơ đồ khi chúng giúp người đọc hiểu cách kiểm chứng.
- Không phóng đại scope hoặc vai trò ngoài bằng chứng đã xác nhận.
- Không công khai IP nội bộ, hostname, credential, tenant/app secret, dữ liệu nhân sự, số liệu nội bộ nhạy cảm hoặc diagram proprietary chưa được làm sạch.

## Kết bài

Kết lại bằng một quan sát hoặc bài học còn giá trị sau project. Không cần “nâng tầm” thành triết lý lớn.

Giọng mong muốn:

> Ghi lại từ những trải nghiệm thực tế của mình trong quá trình làm Infrastructure — những câu chuyện vẫn còn tiếp tục.

## Home page

Home page là lời giới thiệu ngắn, không phải một CV thứ hai và cũng không phải brochure tư vấn.

Headline chuẩn:

> Ghi lại những quyết định kỹ thuật, bài học vận hành và góc nhìn từ thực tế.

Context nghề nghiệp `15+ years in Enterprise Infrastructure` được giữ vì nó giải thích chiều dài trải nghiệm, không dùng như một câu khoe thành tích.

## Checklist trước khi publish

Trước khi đưa một bài hoặc một section mới lên site, tự hỏi:

1. Câu này có giống cách một người làm Infra thật sự kể chuyện không?
2. Có từ nào đang làm câu nghe to hơn bản chất của việc đã làm không?
3. Có chi tiết vận hành nào cụ thể hơn để thay cho một câu khái quát không?
4. Claim về vai trò, kết quả và kỹ thuật có được xác nhận không?
5. Nếu bỏ tên vendor đi, bài học kỹ thuật còn đứng vững không?
6. Người đọc có hiểu mình đã kiểm chứng service bằng cách nào không?
7. Nội dung có vô tình lộ thông tin nội bộ không?

Nếu câu trả lời ổn, mới publish.
