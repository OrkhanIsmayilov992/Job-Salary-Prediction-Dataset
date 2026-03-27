# Maaş Proqnozu Layihəsi

## 📌 Layihə haqqında
Bu layihədə işçilərin xüsusiyyətlərinə (təhsil, təcrübə, vəzifə, lokasiya, şirkət ölçüsü və s.) əsasən **maaş proqnozu** modeli qurulmuşdur. Həm reqressiya (dəqiq maaş), həm də klasifikasiya (yüksək/aşağı maaş) modelləri sınaqdan keçirilmişdir.

## 📊 Dataset
- **Mənbə:** Kaggle - Job Salary Prediction Dataset
- **Sətir sayı:** 250,000
- **Feature sayı:** 12
- **Hədəf:** Maaş (31,867 - 333,046 AZN)

## 🏆 Ən Yaxşı Model: XGBoost

### Reqressiya (Maaş proqnozu)
| Metrik | Dəyər |
|--------|-------|
| R² | **0.9782** |
| MAE | **4,395 AZN** |
| MAPE | **3.2%** |

### Klasifikasiya (Yüksək/Aşağı maaş)
| Metrik | Dəyər |
|--------|-------|
| Accuracy | **94.69%** |
| Precision | **95.04%** |
| Recall | **94.31%** |
| F1-Score | **94.67%** |
| AUC | **0.9912** |

## 📈 Ən vacib feature-lar
1. **exp_edu** (təcrübə × təhsil səviyyəsi) - **34%**
2. **company_size** (şirkət ölçüsü) - **21%**
3. **location** (lokasiya) - **16%**

## 🔧 Quraşdırma
```bash
pip install -r requirements.txt
