# Hướng dẫn chạy Notebook

Dự án này chứa các Jupyter Notebooks để phân tích dữ liệu. Để chạy các notebook, bạn cần tạo môi trường ảo (virtual environment) và cài đặt các thư viện cần thiết.

## Yêu cầu

- Python 3.7 trở lên
- pip (thường đi kèm với Python)

## Các bước cài đặt

### 1. Tạo Virtual Environment

#### Trên Windows:
```powershell
python -m venv venv
```

#### Trên macOS/Linux:
```bash
python3 -m venv venv
```

### 2. Kích hoạt Virtual Environment

#### Trên Windows (PowerShell):
```powershell
.\venv\Scripts\Activate.ps1
```

#### Trên Windows (Command Prompt):
```cmd
venv\Scripts\activate.bat
```

#### Trên macOS/Linux:
```bash
source venv/bin/activate
```

Sau khi kích hoạt, bạn sẽ thấy `(venv)` ở đầu dòng lệnh.

### 3. Cài đặt các thư viện cần thiết

```bash
pip install -r requirements.txt
```

Lệnh này sẽ cài đặt các thư viện sau:
- pandas
- numpy
- matplotlib
- seaborn
- jupyter (nếu chưa có)

### 4. Cài đặt Jupyter Notebook (nếu chưa có)

```bash
pip install jupyter notebook
```

## Chạy Notebook

### Khởi động Jupyter Notebook

```bash
jupyter notebook
```

Hoặc nếu bạn muốn sử dụng JupyterLab:

```bash
jupyter lab
```

Trình duyệt sẽ tự động mở và hiển thị giao diện Jupyter. Bạn có thể mở các notebook:
- `EDA.ipynb`
- `Nhom_10.ipynb`

### Tắt Virtual Environment

Khi hoàn thành công việc, bạn có thể tắt virtual environment bằng lệnh:

```bash
deactivate
```

## Lưu ý

- Luôn kích hoạt virtual environment trước khi chạy notebook
- Nếu gặp lỗi khi cài đặt, hãy đảm bảo bạn đã kích hoạt virtual environment
- Trên Windows PowerShell, nếu gặp lỗi về execution policy, chạy lệnh:
  ```powershell
  Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
  ```

## Cấu trúc dự án

```
DM/
├── EDA.ipynb              # Notebook phân tích dữ liệu khám phá
├── Nhom_10.ipynb          # Notebook nhóm 10
├── DatingAppDataset.csv   # Dataset
├── requirements.txt       # Danh sách thư viện cần thiết
└── venv/                  # Virtual environment (không commit vào git)
```

