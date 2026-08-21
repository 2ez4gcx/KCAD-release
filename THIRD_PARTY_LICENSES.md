# KCAD — Ghi chú giấy phép bên thứ ba

KCAD sử dụng các thư viện dưới đây. Bản phân phối KCAD KHÔNG kèm mã nguồn
KCAD; các thư viện bên thứ ba giữ nguyên giấy phép gốc của chúng.

## Qt 6 / PySide6 — LGPL v3
Giao diện KCAD dựng trên Qt 6 qua binding PySide6 (The Qt Company),
cấp phép **GNU Lesser General Public License v3**. KCAD liên kết ĐỘNG:
các file DLL Qt6*/PySide6 nằm riêng trong thư mục cài và có thể được
thay thế bằng bản Qt tương thích do người dùng tự dịch — đúng điều kiện
LGPL. Văn bản giấy phép: https://www.gnu.org/licenses/lgpl-3.0.html
Mã nguồn Qt: https://code.qt.io/ · PySide6: https://code.qt.io/cgit/pyside/pyside-setup.git

## Các thư viện Python (giấy phép thoáng)
| Thư viện | Giấy phép | Nguồn |
|---|---|---|
| ezdxf | MIT | https://github.com/mozman/ezdxf |
| NumPy | BSD-3-Clause | https://numpy.org |
| Shapely (+GEOS) | BSD-3-Clause | https://github.com/shapely/shapely |
| pymongo/bson | Apache-2.0 | https://github.com/mongodb/mongo-python-driver |
| zstandard | BSD-3-Clause | https://github.com/indygreg/python-zstandard |
| manifold3d | Apache-2.0 | https://github.com/elalish/manifold |
| pybind11 (build lõi C++) | BSD-3-Clause | https://github.com/pybind/pybind11 |
| Python 3.13 runtime | PSF License | https://www.python.org |

Bản đóng gói được biên dịch bằng **Nuitka** (Apache-2.0) — công cụ build,
không áp giấy phép lên sản phẩm đầu ra.

## Những thứ KHÔNG kèm theo — người dùng tự cài
- **ODA File Converter** (Open Design Alliance): cần cho mở/lưu DWG.
  Giấy phép ODA cấm phân phối lại — hãy tự tải từ
  https://www.opendesign.com/guestfiles/oda_file_converter và trỏ đường
  dẫn trong KCAD (Công cụ ▸ Cài đặt ODA File Converter…).
- **Font SHX/TTF** (romans.shx, vnsimli.shx, arial.ttf…): tài sản của
  Autodesk/Microsoft/bên thứ ba, không được phân phối lại. KCAD tự tìm
  font trên máy (thư mục Fonts của AutoCAD, registry Windows, hoặc đặt
  vào thư mục `Fonts` cạnh KCAD.exe do bạn tự chuẩn bị).

## Thương hiệu
AutoCAD® là thương hiệu của Autodesk, Inc. KCAD là phần mềm độc lập,
không liên kết, không bảo trợ bởi Autodesk; tên AutoCAD chỉ xuất hiện
trong tài liệu để mô tả tính tương thích định dạng/thao tác.
