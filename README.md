# KCAD

Phần mềm CAD 2D/3D cho Windows — vẽ kỹ thuật, mở/lưu **DXF, DWG**, in PDF
đúng tỉ lệ, hỗ trợ AutoLISP, giao diện Tiếng Việt / English.

KCAD is a 2D/3D CAD application for Windows — technical drafting with
**DXF/DWG** support, scaled PDF plotting, AutoLISP routines, and a
Vietnamese/English interface.

> Đây là kênh **phát hành bản dùng** (binary release). Repo này không chứa
> mã nguồn.

## Tải về & cài đặt

1. Vào tab **[Releases](../../releases)**, tải file `KCAD-vX.Y.Z-win64.zip`
   mới nhất.
2. Giải nén ra một thư mục bất kỳ (ví dụ `D:\KCAD`).
3. Chạy `KCAD.exe`. Không cần cài Python hay bất kỳ phần mềm nào khác.

> **Windows SmartScreen**: bản phát hành hiện chưa ký số, lần chạy đầu
> Windows có thể hiện "Windows protected your PC" — bấm **More info ▸
> Run anyway**. Phần mềm sạch, toàn bộ được đóng gói từ mã đã biên dịch.

## Hai thứ cần cài thêm (tuỳ nhu cầu)

- **Mở/lưu DWG** — cài [ODA File Converter](https://www.opendesign.com/guestfiles/oda_file_converter)
  (miễn phí, của Open Design Alliance; giấy phép của họ không cho phép
  chúng tôi đóng kèm). Cài xong trỏ đường dẫn trong KCAD:
  *Tệp ▸ Cài đặt ODA File Converter…* (gần cuối menu **Tệp**, dưới *Bảng bút in*).
  File **DXF mở được ngay**, không cần bước này.
- **Font SHX** (chữ kỹ thuật kiểu CAD, gồm font Việt vnsimli/vntimeh…) —
  đây là tài sản của bên thứ ba nên không đóng kèm. Máy đã cài AutoCAD
  thì KCAD tự tìm thấy; nếu không, chép các file `.shx` bạn có bản quyền
  sử dụng vào thư mục `Fonts` đặt cạnh `KCAD.exe`.

## Tính năng chính

- Bộ lệnh vẽ/sửa quen thuộc với người dùng CAD (LINE, PLINE, TRIM,
  OFFSET, FILLET, BLOCK/BEDIT, HATCH, DIM…), bắt điểm 13 mode, grip.
- Mở lại hồ sơ đã từng mở gần như tức thì (cache thông minh); pan/zoom
  mượt trên hồ sơ hàng chục nghìn đối tượng.
- Layout/viewport, in PDF vector đúng tỉ lệ, PUBLISH nhiều tờ, bảng bút .ctb.
- AutoLISP: thả file `.lsp` vào thư mục `Lisp` cạnh exe là tự nạp.
- 3D cơ bản: EXTRUDE/REVOLVE/SWEEP/LOFT, boolean, mặt cắt, FLATSHOT, STL.
- Chữ Việt: Unicode, TCVN3/VNI (lệnh VNFIX chuyển mã), font SHX Việt.

## Giấy phép sử dụng

**Freeware** — được sử dụng miễn phí cho mục đích cá nhân và công việc.
KHÔNG được bán lại, phân phối lại có thu phí, hoặc dịch ngược phần mềm.
Mọi quyền đối với KCAD được bảo lưu bởi tác giả.

Phần mềm cung cấp **NGUYÊN TRẠNG (AS IS)**, không kèm bất kỳ bảo đảm
nào; người dùng tự chịu trách nhiệm kiểm tra kết quả bản vẽ/số liệu
trước khi sử dụng vào công việc thực tế.

Thư viện bên thứ ba và giấy phép của chúng: xem
[THIRD_PARTY_LICENSES.md](THIRD_PARTY_LICENSES.md).

AutoCAD® là thương hiệu của Autodesk, Inc. KCAD là phần mềm độc lập,
không liên kết với Autodesk; tên định dạng DXF/DWG chỉ dùng để mô tả
tính tương thích.

## Báo lỗi

Mở [Issue](../../issues) kèm ảnh chụp màn hình và (nếu được) file DXF
tái hiện lỗi. Vui lòng không đính kèm hồ sơ có thông tin nhạy cảm.
