# PPWL 11/Monorepo - AWS Teams (Tim 1)


## Kelas A / Tim 2
| Nama | NIM | Job |
|------|-----|-----|
| Arjun Maheswara Paundra  | H1101241029 | Admin                  |
| Aurellya Yocelyn Prasista| H1101241043 | Budget & Cost          |
| Febryanti Khumairoh      | H1101241006 | RDS Database           |
| Marcello Chrisdiantoro   | H11012410xx | Lambda Backend         |
| Regisha Sheren           | H1101241036 | S3+CloudFront Frontend |

## Canva - Arsitektur Diagram AWS
🔗 [Link Diagram Arsitektur (Canva Papan Tulis)](https://canva.link/xxxxx)  

### Screenshot wajib:
| Komponen | Screenshot | Status |
|----------|------------|--------|
| S3 Frontend         | [Lihat screenshot](#)    | ✅ |
| RDS Database        | [Lihat screenshot](#)    | ✅ |
| Parameter Store     | [Lihat screenshot](#)    | ✅ |
| Lambda Backend      | [Lihat screenshot](#)    | ✅ |
| CloudFront Frontend | [Lihat screenshot](#)    | ✅ |
| Budget (Monthly)    | [Lihat screenshot](#)    | ✅ |
| Task Cost Report    | [Lihat screenshot](#)    | ✅ |

## Layanan Berjalan & Akses
| Layanan | URL / Endpoint | Status |
|---------|----------------|--------|
| Frontend (CloudFront) | `https://d1keblkrm5z9c0.cloudfront.net/`                                  | ✅ |
| Backend Lambda | `https://zn5qcppmk2j6kbxsckfmk72qvq0pravj.lambda-url.us-east-1.on.aws`           | ✅ |
| RDS PostgreSQL | `postgresql://postgres:tim2ppwl@monorepo-db.cy9qaey8u3kn.us-east-1.rds.amazonaws.com:5432/monorepo_prod` | ✅ |
| S3 Bucket (static) | ` http://s3-monorepo-frontend-blackpa.s3-website-us-east-1.amazonaws.com`    | ✅ |

## Report Bug
1. Akun AWS belum terverifikasi untuk membuat CloudFront

Lokasi: AWS Console → CloudFront → Create distribution

Alur sebelum bug:
Login akun
Mencoba membuat CloudFront distribution untuk frontend
Setelah mengisi konfigurasi, muncul error verifikasi akun
Pesan error:
Your account must be verified before you can add new CloudFront resources.

Solusi yang dicoba:
Membuka kasus ke AWS Support via Account and billing support
Menjelaskan bahwa ini untuk tugas kuliah (university project)
Menyertakan error message dan region yang digunakan (us-east-1).

Selain itu:
Meminta bantuan dari kelompok lain yang akun AWS-nya sudah terverifikasi untuk membuat CloudFront distribution.
Dari CloudFront itu semua request frontend ke backend Lambda menjadi HTTPS, CORS terselesaikan, dan aplikasi berjalan normal. 