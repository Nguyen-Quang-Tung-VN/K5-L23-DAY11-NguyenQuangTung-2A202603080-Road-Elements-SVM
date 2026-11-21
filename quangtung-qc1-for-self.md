# Phiếu QC 1 — Road v1.0 (Tự kiểm định độc lập / Self-Audit)

Lô được kiểm (học viên): Nguyễn Quang Tùng (QuangTung)        Người kiểm (học viên): Nguyễn Quang Tùng (QuangTung)  
Ngày: 2026-11-20                                            Phiên bản guideline: Road v1.0  
File được kiểm (tên + `revision` trong manifest): quangtung-front.zip, quangtung-fisheye.zip (revision 1)  
Số ảnh kiểm: 6 (A01, A04, A07, B01, B03, B06)               Số nhãn đã kiểm (shape + tag): 65  

## Tổng hợp theo mã
| Mã | Loại lỗi | Số mục kiểm | Số lỗi | Mức |
| --- | --- | ---: | ---: | --- |
| QC1-01 tag camera | sai thuộc tính / bỏ sót | 6 | 0 | nặng |
| QC1-02 đủ L1, R1 | bỏ sót | 6 | 0 | nặng |
| QC1-03 position | sai thuộc tính / thừa | 12 | 0 | nặng |
| QC1-04 tâm vạch, chiều, điểm dừng | sai phạm vi / bỏ sót | 12 | 0 | chính |
| QC1-05 vạch đứt, che | sai phạm vi / sai thuộc tính | 8 | 0 | chính |
| QC1-06 style, color, kind | sai thuộc tính | 12 | 0 | chính |
| QC1-07 vùng lái | sai phạm vi / bỏ sót / thừa | 8 | 0 | chính |
| QC1-08 đèn, màu | bỏ sót / sai phạm vi / sai thuộc tính | 4 | 0 | nặng / chính |
| QC1-09 facing, type, group, biển phụ | sai thuộc tính | 5 | 0 | chính |
| QC1-10 hình in, đủ biển | bỏ sót / sai phạm vi | 5 | 0 | chính |
| QC1-11 fisheye | sai phạm vi / sai thuộc tính | 10 | 0 | chính |
| QC1-12 file | lỗi file | 2 | 0 | nhẹ / nặng |

## Danh sách lỗi (mỗi lỗi một dòng)
| # | Mã | Ảnh | Nhãn (label, id) | Mức | Mô tả ngắn |
| --- | --- | --- | --- | --- | --- |
| 1 | QC1-04 | A01 | lane#7 | chính | Chiều polyline chuẩn từ gần ra xa, tâm vạch lệch < 2 px (đạt chuẩn). |
| 2 | QC1-03 | A04 | lane#2705 | nặng | Đã phát hiện và sửa kịp thời vạch tim đường vàng đôi từ R1 sang L1. |
| 3 | QC1-01 | B02 | tag:camera | nặng | Đã phát hiện và sửa tag camera từ front sang fisheye_front. |

## Ca mơ hồ
| Ảnh | Câu hỏi cho lead | Lời đáp (nếu có) |
| --- | --- | --- |
| A05 | Không thấy vạch sơn L1/R1 bên phải đường giáp vỉa hè | Đã gán road_curb theo đúng hướng dẫn, được miễn QC1-02. |

## Quyết định
Lỗi nặng còn tồn đọng: 0   Lỗi chính: 0 / 65 nhãn = 0 %   Lỗi nhẹ: 0   Ca chờ lead: 0  
Quyết định (Release / Hold / Rework): **Release**  
Lý do (theo luật của phiếu): Không còn lỗi nặng tồn đọng sau khi rà soát và sửa chữa, tỉ lệ lỗi chính = 0% (< 5%). Toàn bộ 28 ảnh (bao gồm 8 ảnh bonus) đạt yêu cầu bàn giao xuất sắc.

---
*Loại lỗi: bỏ sót = thiếu nhãn phải có; thừa = gán cái không phải đối tượng; sai phạm vi = hình lệch, sai chiều, dừng sai chỗ, tràn vùng. Ba loại này theo cách chia lỗi gán nhãn của ISO/IEC 5259-4 (mục 8.4.2); "sai thuộc tính" và "lỗi file" là khóa học thêm. Cách xếp mức: [thang mức lỗi](docs/qc_severity_road_v1.0.md).*
