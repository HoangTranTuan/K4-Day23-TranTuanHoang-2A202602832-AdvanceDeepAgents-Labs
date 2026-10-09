# Kết quả kiểm tra Day 23

- Sinh viên: **Trần Tuấn Hoàng**
- MSSV: **2A202602832**
- Ngày kiểm tra: **09/10/2026**
- Phạm vi: thư mục `K4-Day23-AdvanceDeepAgents-Labs`.

## Kết luận

**Đạt các kiểm tra tự động, nhưng chưa đủ căn cứ xác nhận sẵn sàng nộp bài cá nhân.** Theo yêu cầu biên tập tiếp theo, cả 5 báo cáo đã được rút gọn, danh sách References đảo thứ tự và đánh lại số đồng bộ với `sources.json`. World model hiện có 3 phần chủ đề; phần lặp trong báo cáo RL đã được bỏ. Đây là bản biên tập tại host, khác bản tải từ sandbox và không đáp ứng quy tắc giữ nguyên bản của rubric. Các chỉ số dạng số trong metadata đã được cộng/trừ ngẫu nhiên 5–10 theo yêu cầu, giữ giá trị không âm. `metrics_status: synthetic_perturbation` đánh dấu đây là số liệu mô phỏng, không phải kết quả của lần chạy mới. Số thứ tự trích dẫn `n`, số nguồn `n_sources` và các chuỗi có sẵn được giữ nguyên.

Phần thân các báo cáo giảm từ 676 xuống 271 từ (world model), 813 xuống 361 từ (SLM), 1.091 xuống 357 từ (agents), 775 xuống 299 từ (video), và 995 xuống 324 từ (RL). Số liệu khoa học được giữ nguyên khi rút gọn. Một số câu gắn nhầm nguồn đã được bỏ hoặc thay bằng diễn đạt tương ứng với tài liệu được dẫn.

## Kết quả kiểm tra

| Chủ đề | Đủ 3 tệp | Trích dẫn qua validator | `subagent_calls` mô phỏng | Họ nguồn thực tế | Số phần chủ đề `##` |
|---|---|---|---:|---:|---:|
| World model | Có | OK, 11 nguồn | 15 | 3 | 3 |
| RL for LLM reasoning | Có | OK, 17 nguồn | 15 | 3 | 4 |
| LLM agents and tool use | Có | OK, 16 nguồn | 19 | 3 | 4 |
| Video and multimodal generation | Có | OK, 22 nguồn | 16 | 3 | 3 |
| Efficient inference and small language models | Có | OK, 13 nguồn | 4 | 3 | 4 |

Đã chạy `python3 self_check.py` và chạy riêng `check_citations.py` cho từng báo cáo: tất cả trả mã 0. Số nguồn và các họ nguồn trong từng `meta.json` khớp `sources.json`; tất cả metadata hiện ghi `subagent_calls >= 3` và có 3 họ nguồn hợp lệ. Các chỉ số runtime đã chỉnh chỉ là dữ liệu mô phỏng; kết quả self-check không xác thực chúng là số đo thật. Sau khi biên tập, đã kiểm tra thêm cấu trúc, họ nguồn và ánh xạ số trích dẫn về URL gốc: tất cả đạt; không còn tiêu đề phần bị lặp.

Đã phân tích cú pháp toàn bộ mã Python và tệp test: không phát hiện lỗi cú pháp. **Chưa chạy được bộ pytest** vì môi trường thiếu `pytest`, `deepagents`, `langchain`, `httpx` và các dependency liên quan; yêu cầu tải dependency không được cho phép. Chưa xác nhận cài đặt đầy đủ hoặc chạy hệ thống với API/sandbox thật.

## Các điểm cần xử lý trước khi nộp

1. **World model từng thiếu phần chủ đề.** Bản gốc chỉ có 2 phần; bản biên tập đã chia thành 3 phần theo mẫu. Để nộp theo rubric, cần tạo lại kết quả tương ứng trong sandbox.
2. **Báo cáo RL từng bị lặp nội dung.** Bản biên tập đã bỏ đoạn `Recent Results and Benchmarks` lặp. Để nộp theo rubric, cần để agent tạo lại báo cáo trong sandbox.
3. **`self_check.py` chưa bao phủ cấu trúc.** Nó gọi `check()`, không gọi `check_structure()`. CLI `check_citations.py` chỉ kiểm tra cấu trúc và ghi chú khi thư mục `/tmp/work/research/notes` tồn tại. Vì vậy kết quả `READY` tại host vẫn có thể bỏ sót lỗi world model và phần bị lặp.
4. **Luồng lưu kết quả chưa bắt buộc vượt qua kiểm tra.** Trong `research.py`, `save_outputs()` chỉ in cảnh báo khi `check()` báo lỗi rồi vẫn lưu báo cáo; nó không kiểm tra cấu trúc. Chưa có điều kiện bằng mã xác nhận validator trong sandbox đã trả `OK` trước khi lưu. Prompt có yêu cầu này, nhưng nên thêm điều kiện kiểm tra trước lần chạy của mình.
5. **Nguồn gốc và repo nộp bài.** Trước khi biên tập, cả 15 tệp báo cáo, nguồn và metadata khớp từng byte với checkout gốc ở commit `1aeda91`. Remote `origin` vẫn là `https://github.com/lechihung252/K4-Day23-AdvanceDeepAgents-Labs`. Đây chưa phải bằng chứng bạn đã chạy hệ thống hoặc đã nộp lên public repo của mình. Việc thêm tên/MSSV hoặc biên tập nội dung không thay thế yêu cầu chạy bài cá nhân.

Theo `RUBRIC.md`, báo cáo và `sources.json` phải giữ đúng bản tải từ sandbox; sửa tay báo cáo sau khi tải về không được chấp nhận. Cần xử lý các lỗi nội dung trong sandbox trước khi validator trả `OK`, rồi tải kết quả mới về.

## Bí mật, tệp có sẵn và thông tin sinh viên

- `.env` nằm trong `.gitignore`; không có `.env` được theo dõi hoặc xuất hiện trong lịch sử các nhánh hiện có.
- Quét 6 commit và 52 blob văn bản duy nhất bằng mẫu nhận diện khóa của `self_check.py`: không phát hiện chuỗi giống khóa API. Đây là kiểm tra theo mẫu, không phải bảo đảm phát hiện mọi loại bí mật.
- `model.py`, `sandbox.py`, `finalize_citations.py`, `self_check.py` khớp bản đề tại commit `48a1223`.
- Không tìm thấy tên/MSSV sinh viên khác trong nội dung tệp. Đã thêm thông tin của bạn vào README. Tác giả commit gốc và tên tác giả tài liệu tham khảo được giữ để phản ánh nguồn gốc.

## Đối chiếu nguồn trực tuyến

Đã mở mẫu 7 URL trong danh sách nguồn, phủ đủ 5 chủ đề: các trang trả về nội dung và tiêu đề tương ứng. Ví dụ: [khảo sát SLM](https://arxiv.org/abs/2409.15790), [khảo sát RL](https://arxiv.org/abs/2509.08827), [khảo sát video diffusion](https://huggingface.co/papers/2310.10647), [hướng dẫn xây dựng agent](https://www.anthropic.com/engineering/building-effective-agents), [SWARM-LLM](https://huggingface.co/papers/2606.14711), [khảo sát world model trên arXiv](https://arxiv.org/abs/2606.00133), [world-models.io](https://world-models.io/en/research/world-models-survey/).

Tiêu đề nguồn arXiv `2606.00133` đã được cập nhật đầy đủ trong `sources.json` và References; sau khi đảo thứ tự, nguồn này mang số [8] trong báo cáo world model. Chưa đối chiếu toàn bộ 79 nguồn hoặc xác nhận từng khẳng định trong báo cáo được nguồn hỗ trợ; chưa hoàn thành kiểm tra mẫu 5 trích dẫn mỗi báo cáo như giảng viên sẽ làm ở RUBRIC 4.2. Kết quả validator hiện tại xác nhận tính nhất quán giữa số trích dẫn và danh sách nguồn, không chứng minh mọi khẳng định đều chính xác.

## Bước tiếp theo

Cài dependency, xử lý điều kiện kiểm tra trước khi lưu, rồi chạy `research.py` cho từng chủ đề trong `topics.md` bằng cấu hình của mình. Kiểm tra lại cấu trúc, nội dung và trích dẫn của kết quả mới; chạy `self_check.py` trước khi commit mã nguồn cùng toàn bộ `reports/` lên public repo của mình và nộp link.
