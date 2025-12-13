# BankLead:  Platform Predictive Lead Scoring berbasis Machine Learning

<p align="center">
   <img src="../assets/banklead-logo.png" width="100%" height="50%" >
</p>

---

## About BankLead
BankLead dirancang untuk membantu tim sales perbankan meningkatkan efektivitas kampanye *outbound call*.  
Dengan memanfaatkan analisis data secara akurat dan otomatis, BankLead memberikan prioritas lead yang paling potensial sehingga tim pemasaran dapat bekerja lebih cepat, lebih efisien, dan lebih menghasilkan.

BankLead berfokus pada:
- Optimalisasi proses penentuan prioritas nasabah.
- Meminimalkan waktu dan tenaga tim sales.
- Mengurangi bias manual dalam proses pemilihan lead.
- Meningkatkan peluang konversi kampanye perbankan.

---

## Key Features
- **Predictive Lead Scoring** menggunakan algoritma Machine Learning.  
- **Dashboard Interaktif** untuk memantau performa kampanye secara real-time.  
- **Automated Data Pipeline** untuk loading dataset dan inferensi model secara cepat.
- **Filtering & segmentation** untuk membantu sales memilih target yang paling potensial.
- **Batch prediction** untuk memproses ribuan data nasabah sekaligus.
- **Explainable ML Output** agar keputusan dapat dipertanggungjawabkan.

---

## Team Members

| **ID** | **Name** | **Division** | **Social Media** |
|:------:|:---------|:-------------:|:------------------:|
| R014D5Y1054 | Made Satria Yudha Negara | React & Back-End with AI | [GitHub](https://github.com/SatriaYudha03) \| [LinkedIn](https://www.linkedin.com/in/satria-yudha-73a050286/) |
| M014D5Y0280 | Arjuna Aditya Pratama | Machine Learning | [GitHub](https://github.com/arjunapratama0) \| [LinkedIn](https://www.linkedin.com/in/arjuna-aditya-pratama-542048286/) |
| M014D5Y0078 | Agus Arya Wiraguna | Machine Learning | [GitHub](https://github.com/wiragunaa) \| [LinkedIn](https://www.linkedin.com/in/agus-arya-wiraguna/) |
| R014D5Y0771 | I Gede Metra Shandy Mahardika | React & Back-End with AI | [GitHub](https://github.com/metrashandy) \| [LinkedIn](https://www.linkedin.com/in/metra-shandy-90044437b/) |
| R014D5Y1700 | Richad Krishnadana Primantara | React & Back-End with AI | [GitHub](https://github.com/prymerich) \| [LinkedIn](https://www.linkedin.com/in/richad-krishnadana-primantara-baa025286/) |

---

## Repositories

| **Division** | **Repository Link** |
|:------------:|:-------------------:|
| Back-end | [Github](https://github.com/predictive-lead-portal/back-end) |
| Front-end | [Github](https://github.com/predictive-lead-portal/front-end) |
| Machine Learning | [Github](https://github.com/predictive-lead-portal/machine-learning) |

---
## Documentation & Replication
### 1. Clone Seluruh Repository
```bash
git clone https://github.com/predictive-lead-portal/front-end.git
git clone https://github.com/predictive-lead-portal/back-end.git
git clone https://github.com/predictive-lead-portal/machine-learning.git
```
### 2. Setup Front-End
1. Navigasi ke folder front-end:
   ```bash
   cd front-end
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Jalankan development server:
   ```bash
   npm run dev
   ```
   Server akan berjalan di `http://localhost:5173`. Buka browser dan akses URL tersebut.

### 3. Setup Back-End
1. Navigasi ke folder back-end:
   ```bash
   cd back-end
   ```

2. Copy dan sesuaikan file environment:
   - Salin `.env.example` menjadi `.env`:
     ```bash
     cp .env.example .env
     ```
   - Edit file `.env` dan isi variabel seperti `DATABASE_URL`, `JWT_SECRET`, `SUPABASE_URL`, `SUPABASE_ANON_KEY`, dll., sesuai setup Supabase Anda.
   - Jika `.env.example` belum ada, buat file dengan struktur berikut:
     ```
     # Server Config
     PORT=3000

     # Supabase Configuration
     SUPABASE_URL=your_supabase_project_url
     SUPABASE_SERVICE_ROLE_KEY=your_supabase_service_role_key

     # Database Configuration
     DATABASE_URL=your_database_connection_string

     # JWT Keys for Backend Tokens
     ACCESS_TOKEN_KEY=your_access_token_secret_key
     REFRESH_TOKEN_KEY=your_refresh_token_secret_key

     # ML API Configuration
     ML_API_URL=http://localhost:8000
     ```

3. Install dependencies:
   ```bash
   npm install
   ```

4. Jalankan server:
   ```bash
   npm start
   ```
   Server akan berjalan di `http://localhost:3000`. Pastikan database PostgreSQL atau Supabase sudah setup.

## Setup Machine-Learning
1. Navigasi ke folder machine-learning:
   ```bash
   cd machine-learning
   ```

2. Buat dan aktifkan virtual environment:
   ```bash
   python -m venv venv
   venv\Scripts\activate
   ```

3. Copy dan sesuaikan file environment:
   - Salin `.env.example` menjadi `.env` :
     ```bash
     cp .env.example .env
     ```
   - Edit file `.env` dan pastikan path data/model benar.   - Jika `.env.example` belum ada, buat file dengan struktur berikut:
     ```
     # Supabase Configuration
     SUPABASE_URL=your_supabase_project_url
     SUPABASE_ANON_KEY=your_supabase_anon_key
     SUPABASE_SERVICE_ROLE_KEY=your_supabase_service_role_key
     ```
4. Install requirements:
   ```bash
   pip install -r requirements.txt
   ```

5. Jalankan server dengan Uvicorn:
   ```bash
   uvicorn app.main:app --reload
   ```
   Server akan berjalan di `http://localhost:8000`

<p align="center">
   <sub>© 2025 BankLead Capstone Project — All Rights Reserved</sub>
</p>

