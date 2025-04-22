# 📝 Pylog - Django 기반 블로그 프로젝트

[![Python Version](https://img.shields.io/badge/Python-3.11+-blue.svg)](https://www.python.org/)
[![Django](https://img.shields.io/badge/Django-4.x-green.svg)](https://www.djangoproject.com/)

## 🔍 소개

**Pylog**는 Django 프레임워크로 제작된 개인 블로그 웹 애플리케이션입니다.  
게시글 CRUD, 이미지 업로드, 기본 스타일링을 지원하며 학습 또는 포트폴리오 용도로 활용할 수 있습니다.

---

## 🧩 주요 기능

- 📄 게시글 등록, 수정, 삭제
- 🖼️ 썸네일 이미지 업로드
- 🧭 기본 템플릿 및 정적 파일 구성
- 🗂️ Django admin 기반 관리 기능

---

## 📁 프로젝트 구조

```
📁 Pylog-master/
├── 📁 blog/                      # 블로그 앱
│   ├── admin.py, models.py, views.py
│   ├── migrations/              # DB 마이그레이션
│   └── templates/               # post 템플릿 포함
│
├── 📁 config/                    # Django 설정
│   ├── settings.py, urls.py, wsgi.py
│
├── 📁 static/                    # 정적 파일(css)
│   └── css/style.css
│
├── 📁 media/                     # 업로드 이미지
│   └── post/xxx.jpg
│
├── 📁 templates/                 # 메인 템플릿
│   ├── index.html, post_list.html 등
│
├── 📄 manage.py
└── 📄 db.sqlite3
```

---

## 🚀 실행 방법

```bash
git clone https://github.com/yourusername/pylog.git
cd pylog

python -m venv venv
source venv/bin/activate
pip install -r requirements.txt  # 필요 시 수동 생성

python manage.py makemigrations
python manage.py migrate
python manage.py runserver
```

👉 브라우저에서 `http://127.0.0.1:8000` 접속

---

## 📌 추가 정보

- 관리자 계정 생성: `python manage.py createsuperuser`
- 게시글 템플릿: `post_list.html`, `post_detail.html` 등
- 미디어/정적 파일은 개발환경 기준으로 구성됨

