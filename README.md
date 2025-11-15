# 👋 Đặng Trần Thành  
### Credit Risk Modeling • Banking Risk Analytics  

Git này bao gồm các nội dung xây dựng các mô hình **chấm điểm tín dụng (Credit Scoring)**, thiết kế **MoE architectures** cho mô hình PD, và phát triển **synthetic scenario** để kiểm thử rủi ro trong môi trường ngân hàng & fintech.  
Kết hợp kinh nghiệm Data Science với các chuẩn thực tế của ngành như **COSO ERM 2017**, **Basel II/III**, và **Model Governance**.

---

## Key Expertise

### Credit Risk Modeling
- **Segmentation (CHAID/CART):** chia khách hàng thành các nhóm rủi ro đồng nhất trước khi mô hình hóa.  
- **Logistic Regression Scorecard:** mô hình truyền thống, dễ giải thích; sử dụng WOE/Binning + PD calibration.  
- **Random Forest Benchmark:** kiểm tra phi tuyến, đo tầm quan trọng biến, hỗ trợ cải thiện mô hình chính.  
- **Interpretability & Monitoring:** SHAP/PDP + KS/Gini/PSI để giải thích kết quả và theo dõi độ ổn định mô hình.  

### Mixture-of-Experts (MoE) for Credit Scoring
- **Expert thiết kế theo phân phối khách hàng thực tế:** mô hình tách khách hàng thành nhóm *có lịch sử tín dụng đầy đủ*, *thiếu lịch sử*, và *không có lịch sử* (thin-file/no-file) để chuyên biệt hóa rủi ro.
  - **Application Expert:** demographics, income, employment – hiệu quả cho khách hàng mới hoặc thiếu dữ liệu.  
  - **Behavioral Expert:** transaction behavior, spending patterns, utilization – dành cho khách hàng có lịch sử hành vi đủ dài.  
  - **Bureau Expert:** external credit history, inquiry patterns – giải quyết nhóm có CIC/credit bureau mạnh.  
  - **Alt-Data Expert:** dữ liệu thay thế (telco, e-wallet, utility, device fingerprint) cho khách hàng **không có** lịch sử tín dụng truyền thống.  
- **Gating Network:** tự động nhận diện đặc điểm hồ sơ và phân bổ trọng số cho expert phù hợp → cải thiện accuracy cho cả *full-file* và *thin-file/no-file*.  
- **LLM + RAG Explainability:** sinh giải thích mô hình theo từng khách hàng dựa trên đặc điểm dữ liệu và expert được kích hoạt.

### Synthetic Data & Scenario Testing
- Tạo dữ liệu tín dụng giả lập (income, DTI, delinquency, loan history) phản ánh cấu trúc thị trường Việt Nam (vay tiêu dùng, vay thế chấp, SME…).  
- Stress Testing phù hợp bối cảnh Việt Nam:
  - **Macro downturn:** tăng lãi suất, giảm thu nhập, suy giảm ngành BĐS/SME.  
  - **Portfolio deterioration:** nợ xấu tăng theo phân khúc (vay tiêu dùng, BĐS, hộ kinh doanh).  
  - **Probability-of-default shift:** thay đổi PD theo chính sách siết room tín dụng, hạn mức LTV/DTI, chất lượng thu hồi nợ.  

### Risk Monitoring & Reporting
- NPL, PAR30/90, Vintage, Migration matrix  
- KRI framework + Risk Appetite  
- Dashboard Power BI / Excel  
- Portfolio drift (PSI), stability check  

### Risk Governance
- COSO ERM 2017  
- Basel II/III (PD/LGD/EAD concepts)  
- Model Lifecycle: Development → Validation → Monitoring  
- Data quality controls

---
