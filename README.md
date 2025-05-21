## 🎯 Learning Goals

- Build a multi-user file upload portal
- Handle file input securely with size/type validation
- Store files in organized per-user directories
- Audit common upload vulnerabilities

## 🔐 Security Audit Focus

- ❌ No MIME type verification
- ❌ Dangerous extensions accepted (.php, .sh, .bat)
- ❌ Unlimited file size upload
- ✅ Bonus: ClamAV or simulated file scanning
- ✅ Bonus: User-only file visibility

See [`audit-checklist.md`](./audit-checklist.md) for details.

## ✅ Features

- Upload, list, and delete files
- Only logged-in users can upload/view their own files
- File validation: type, extension, size
- Optional scan with ClamAV or mock logic
- Organized file storage per user

## 🤝 Contributions
Pull requests are welcome! If you’d like to add features, improve security hardening, optimize code, or extend functionality, feel free to open an issue or PR. This is a learning-focused lab project, and collaboration is encouraged.


## 🚀 Getting Started

```bash
git clone https://github.com/yourusername/django-file-upload-secured.git
cd django-file-upload-secured
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver


