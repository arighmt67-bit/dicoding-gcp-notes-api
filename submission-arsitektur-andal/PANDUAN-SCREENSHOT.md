# Panduan Screenshot Asli Google Cloud Console (Target Bintang 5)

Sesuai aturan anti-fabrikasi Dicoding, screenshot wajib diambil langsung dari antarmuka Google Cloud Console asli (bukan editan/mockup).

Silakan buka Cloud Console di browser dengan akun **arighmt67@gmail.com** dan pastikan project aktif adalah:
**Project Name:** `submission-gca-arirahmatr`  
**Project ID:** `project-183cf8ce-97a2-455e-aad`

---

### 1. Screenshot Project ID / Project Name
* **URL:** `https://console.cloud.google.com/welcome?project=project-183cf8ce-97a2-455e-aad`
* **Nama File:** `screenshots/1_project_id.png`
* **Yang harus terlihat jelas:**
  - Header Cloud Console yang menunjukkan Project Name `submission-gca-arirahmatr` dan Project ID `project-183cf8ce-97a2-455e-aad`.
  - Kartu Project Info di Dashboard.

---

### 2. Screenshot Protokol Load Balancer & Managed Instance Group
* **URL Load Balancer:** `https://console.cloud.google.com/net-services/loadbalancing/loadBalancers/list?project=project-183cf8ce-97a2-455e-aad`
* **Nama File:** `screenshots/2a_load_balancer.png`
* **Yang harus terlihat jelas:**
  - Nama Load Balancer: `ecommerce-http-lb-rule` (atau detail `ecommerce-backend-service`).
  - Protokol: `HTTP`.
  - IP Frontend: `8.232.179.128:80`.
  - Backend Services menunjukkan 2 backend (`mig-asia` & `mig-eu`) dengan status `Healthy`.
* **URL Instance Groups:** `https://console.cloud.google.com/compute/instanceGroups/list?project=project-183cf8ce-97a2-455e-aad`
* **Nama File:** `screenshots/2b_managed_instance_groups.png`
* **Yang harus terlihat jelas:**
  - Dua instance group: `mig-asia` (`asia-southeast2-a`) dan `mig-eu` (`europe-west1-b`).
  - Kolom Autoscaled: `Yes (on)` pada kedua instance group.

---

### 3. Screenshot Custom Dashboard Monitoring
* **URL:** `https://console.cloud.google.com/monitoring/dashboards?project=project-183cf8ce-97a2-455e-aad`
* (Atau klik langsung dashboard `Dashboard - Submission`)
* **Nama File:** `screenshots/3_custom_dashboard.png`
* **Yang harus terlihat jelas:**
  - Judul dashboard: `Dashboard - Submission`.
  - Keempat chart dengan tipe dan metrik bervariasi:
    1. CPU Utilization (Compute Engine)
    2. Network Inbound Traffic (Compute Engine)
    3. Disk Read Bytes (Compute Engine)
    4. Load Balancer Request Count (HTTP LB)

---

### 4. Screenshot IAM Hak Akses Auditor Eksternal (Least Privilege)
* **URL:** `https://console.cloud.google.com/iam-admin/iam?project=project-183cf8ce-97a2-455e-aad`
* **Nama File:** `screenshots/4_iam_reviewer.png`
* **Yang harus terlihat jelas:**
  - Principal: `reviewer_googlecloud@dicoding.com` (tipe Group icon).
  - Role yang tertera (Granular Least Privilege):
    - `Compute Viewer`
    - `Monitoring Viewer`
    - `Browser`

---

### 5. Screenshot VPC Networks (Saran Opsional Bintang 5)
* **URL:** `https://console.cloud.google.com/networking/networks/list?project=project-183cf8ce-97a2-455e-aad`
* **Nama File:** `screenshots/5_vpc_custom_mode.png`
* **Yang harus terlihat jelas:**
  - Nama network: `vpc-ecommerce`.
  - Kolom Subnet creation mode: `Custom`.
  - Subnet terlihat: `subnet-asia-southeast2` (`10.10.0.0/24`) dan `subnet-europe-west1` (`10.20.0.0/24`).

---

### Cara Simpan:
Letakkan kelima file screenshot tersebut ke dalam folder:
`~/projects/a332-google-cloud-architect-labs/submission-arsitektur-andal/screenshots/`
