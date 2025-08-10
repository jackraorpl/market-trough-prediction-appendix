# DML Sensitivity Analysis Report

## Analysis for DML-PLR

### Summary Statistics

-   **Total variables tested:** 228
-   **Number of robust findings:** 27
-   **Number of non-robust findings:** 201

### Robust Causal Estimates (DML-PLR)

| treatment_variable                         |   theta | p_value | adj_conf_int_lower | adj_conf_int_upper |
|:----------------------|------------:|------------:|------------:|------------:|
| ffr_slope_trend_z_scaled_last              | -0.0157 |       0 |            -0.0216 |            -0.0098 |
| ffr_slope_roc63_scaled_last                | -0.0228 |       0 |            -0.0368 |            -0.0087 |
| credit_spread_scaled_std                   | -0.0524 |       0 |            -0.0743 |            -0.0306 |
| credit_spread_trend_z_scaled_std           | -0.0522 |       0 |            -0.0747 |            -0.0297 |
| fx_rv_6j_21d_trend_z_scaled_mean           | -0.0143 |       0 |            -0.0207 |            -0.0078 |
| ffr_slope_roc63_scaled_mean                | -0.0122 |  0.0001 |            -0.0181 |            -0.0062 |
| ffr_slope_scaled_last                      | -0.0154 |  0.0001 |             -0.023 |            -0.0079 |
| amihud_illiquidity_trend_z_scaled_std      | -0.0608 |  0.0001 |            -0.0917 |            -0.0299 |
| ffr_slope_scaled_mean                      | -0.0145 |  0.0003 |            -0.0224 |            -0.0066 |
| fx_rv_6j_21d_trend_z_scaled_last           | -0.0153 |  0.0005 |            -0.0238 |            -0.0067 |
| ffr_slope_scaled_trend                     | -0.1436 |   0.001 |            -0.2293 |            -0.0579 |
| fx_rv_6j_21d_scaled_mean                   | -0.0128 |  0.0025 |            -0.0248 |            -0.0007 |
| pcr_oi_roc63_scaled_std                    | -0.0549 |  0.0057 |            -0.0938 |             -0.016 |
| risk_neutral_skewness_scaled_trend         | -0.1346 |  0.0069 |            -0.2321 |             -0.037 |
| risk_neutral_skewness_trend_z_scaled_trend | -0.1533 |  0.0082 |            -0.2669 |            -0.0397 |
| flow_concentration_10d_scaled_std          |  0.0636 |  0.0124 |             0.0138 |             0.1134 |
| fx_rv_6j_21d_scaled_last                   | -0.0096 |  0.0135 |            -0.0172 |             -0.002 |
| ffr_basis_roc63_scaled_mean                |  0.0111 |  0.0177 |             0.0019 |             0.0202 |
| risk_neutral_kurtosis_trend_z_scaled_mean  |  0.0186 |  0.0196 |              0.003 |             0.0342 |
| flow_concentration_10d_trend_z_scaled_mean | -0.0093 |  0.0202 |            -0.0172 |            -0.0015 |
| flow_concentration_10d_trend_z_scaled_std  |  0.0404 |  0.0219 |             0.0059 |              0.075 |
| flow_concentration_10d_roc63_scaled_std    |  0.0515 |  0.0228 |             0.0072 |             0.0958 |
| ffr_basis_roc63_scaled_last                |  0.0081 |   0.026 |              0.001 |             0.0152 |
| ffr_slope_trend_z_scaled_trend             | -0.0834 |  0.0306 |             -0.159 |            -0.0078 |
| risk_neutral_kurtosis_scaled_mean          |  0.0173 |  0.0306 |             0.0016 |             0.0329 |
| risk_neutral_skewness_roc63_scaled_trend   | -0.0946 |  0.0359 |            -0.1829 |            -0.0062 |
| pcr_oi_trend_z_scaled_std                  | -0.0337 |   0.042 |            -0.0662 |            -0.0012 |

### Top 10 Notable Non-Robust Findings

| treatment_variable                      |   theta | p_value | is_robust | bias_phi | adj_conf_int_lower | adj_conf_int_upper | benchmark_r2_y | benchmark_r2_d |
|:-------|-------:|-------:|:-------|-------:|-------:|-------:|-------:|-------:|
| realized_volatility_trend_z_scaled_mean |  -0.016 |  0.0011 | False     |   0.3036 |            -0.3293 |             0.2972 |         0.0639 |         0.8449 |
| realized_volatility_roc63_scaled_mean   | -0.0202 |   0.026 | False     |   0.2781 |             -0.316 |             0.2756 |         0.0653 |         0.8277 |
| dex_oi_roc63_scaled_mean                | -0.0106 |  0.0162 | False     |   0.1569 |            -0.1762 |              0.155 |         0.0454 |         0.7751 |
| vix_roc63_scaled_mean                   |  0.0174 |  0.0045 | False     |   0.1582 |            -0.1528 |             0.1876 |          0.049 |         0.7699 |
| vix_trend_z_scaled_last                 |  0.0099 |  0.0232 | False     |   0.1306 |            -0.1292 |              0.149 |          0.049 |         0.7574 |
| vix_roc63_scaled_last                   |  0.0245 |  0.0009 | False     |   0.1277 |            -0.1176 |             0.1666 |         0.0481 |         0.7459 |
| dex_oi_scaled_mean                      | -0.0237 |  0.0014 | False     |   0.1307 |             -0.169 |             0.1215 |         0.0462 |         0.7429 |
| upg_63d_roc63_scaled_mean               | -0.0271 |  0.0001 | False     |   0.1317 |            -0.1728 |             0.1185 |         0.0475 |         0.7414 |
| vix_roc63_scaled_trend                  |  0.2121 |  0.0008 | False     |   1.1103 |            -1.0221 |             1.4463 |         0.0489 |         0.7177 |
| upg_63d_roc63_scaled_last               | -0.0278 |  0.0001 | False     |   0.0972 |            -0.1387 |             0.0831 |         0.0476 |         0.6873 |

## Analysis for DML-APE

### Summary Statistics

-   **Total variables tested:** 228
-   **Number of robust findings:** 48
-   **Number of non-robust findings:** 180

### Robust Causal Estimates (DML-APE)

| treatment_variable                         |   theta | p_value | adj_conf_int_lower | adj_conf_int_upper |
|:----------------------|------------:|------------:|------------:|------------:|
| fx_rv_6j_21d_roc63_scaled_std              |  0.0057 |       0 |             0.0046 |             0.0069 |
| risk_neutral_kurtosis_trend_z_scaled_std   |  0.0485 |       0 |             0.0413 |             0.0557 |
| fx_rv_6j_21d_trend_z_scaled_std            |  0.0072 |       0 |             0.0061 |             0.0083 |
| risk_neutral_kurtosis_roc63_scaled_std     |  0.0382 |       0 |             0.0339 |             0.0425 |
| ffr_slope_trend_z_scaled_std               |  0.0092 |       0 |             0.0083 |               0.01 |
| fx_rv_6e_21d_scaled_std                    |    0.01 |       0 |             0.0089 |              0.011 |
| amihud_illiquidity_trend_z_scaled_std      |   0.016 |       0 |             0.0129 |             0.0191 |
| risk_neutral_skewness_trend_z_scaled_std   |  0.0343 |       0 |             0.0301 |             0.0384 |
| risk_neutral_skewness_scaled_std           |  0.0359 |       0 |              0.032 |             0.0397 |
| risk_neutral_skewness_roc63_scaled_std     |  0.0399 |       0 |              0.032 |             0.0479 |
| pcr_oi_trend_z_scaled_std                  |  0.0213 |       0 |             0.0196 |             0.0231 |
| fx_rv_6e_21d_roc63_scaled_mean             | -0.0016 |       0 |             -0.002 |            -0.0012 |
| ffr_slope_roc63_scaled_std                 |  0.0063 |       0 |             0.0057 |              0.007 |
| pcr_oi_scaled_std                          |  0.0191 |       0 |             0.0178 |             0.0203 |
| fx_rv_6e_21d_roc63_scaled_std              |  0.0061 |       0 |             0.0048 |             0.0074 |
| pcr_oi_roc63_scaled_std                    |  0.0241 |       0 |             0.0214 |             0.0268 |
| ffr_slope_scaled_std                       |  0.0103 |       0 |             0.0099 |             0.0107 |
| ffr_slope_scaled_last                      |  0.0177 |       0 |             0.0146 |             0.0209 |
| fx_rv_6j_21d_scaled_std                    |  0.0051 |       0 |             0.0039 |             0.0063 |
| risk_neutral_kurtosis_scaled_std           |  0.0957 |       0 |             0.0726 |             0.1189 |
| fx_momentum_6e_21d_trend_z_scaled_std      |  0.0047 |       0 |             0.0035 |             0.0058 |
| ffr_slope_scaled_trend                     | -0.0073 |       0 |            -0.0092 |            -0.0054 |
| gex_oi_trend_z_scaled_std                  |  0.0773 |       0 |             0.0381 |             0.1165 |
| fx_momentum_6e_21d_scaled_std              |  0.0038 |       0 |             0.0028 |             0.0049 |
| fx_rv_6j_21d_trend_z_scaled_last           | -0.0018 |       0 |            -0.0023 |            -0.0012 |
| fx_momentum_6j_21d_trend_z_scaled_std      |  0.0026 |       0 |             0.0018 |             0.0035 |
| fx_rv_6e_21d_roc63_scaled_last             | -0.0012 |       0 |            -0.0017 |            -0.0008 |
| ffr_slope_trend_z_scaled_trend             | -0.0066 |       0 |             -0.009 |            -0.0042 |
| fx_rv_6e_21d_trend_z_scaled_mean           | -0.0012 |       0 |            -0.0017 |            -0.0008 |
| fx_rv_6e_21d_trend_z_scaled_last           | -0.0009 |       0 |            -0.0013 |            -0.0006 |
| fx_rv_6j_21d_trend_z_scaled_trend          |  0.0037 |       0 |              0.002 |             0.0054 |
| fx_rv_6j_21d_trend_z_scaled_mean           | -0.0017 |  0.0001 |            -0.0025 |            -0.0009 |
| ffr_slope_roc63_scaled_last                | -0.0006 |  0.0001 |            -0.0009 |            -0.0003 |
| fx_rv_6e_21d_scaled_mean                   | -0.0009 |  0.0003 |            -0.0014 |            -0.0004 |
| flow_concentration_10d_trend_z_scaled_mean | -0.0013 |  0.0003 |            -0.0021 |            -0.0006 |
| risk_neutral_kurtosis_scaled_mean          |  0.0051 |  0.0008 |             0.0021 |             0.0081 |
| fx_rv_6e_21d_trend_z_scaled_trend          |  0.0024 |  0.0009 |              0.001 |             0.0038 |
| flow_concentration_10d_scaled_std          |  0.0021 |  0.0013 |             0.0008 |             0.0034 |
| ffr_basis_roc63_scaled_trend               |  -0.002 |  0.0034 |            -0.0033 |            -0.0006 |
| ffr_slope_scaled_mean                      |  0.0011 |  0.0085 |             0.0003 |             0.0019 |
| ffr_basis_scaled_last                      |  0.0007 |  0.0096 |             0.0002 |             0.0012 |
| vrp_roc63_scaled_std                       | -0.0021 |  0.0099 |            -0.0036 |            -0.0005 |
| flow_concentration_10d_roc63_scaled_std    |  0.0018 |  0.0114 |             0.0004 |             0.0031 |
| risk_neutral_kurtosis_trend_z_scaled_trend |  -0.006 |  0.0233 |            -0.0111 |            -0.0008 |
| ffr_basis_roc63_scaled_last                | -0.0003 |  0.0299 |            -0.0006 |                 -0 |
| risk_neutral_kurtosis_scaled_trend         | -0.0043 |  0.0313 |            -0.0082 |            -0.0004 |
| ffr_basis_scaled_mean                      |  0.0006 |  0.0345 |                  0 |             0.0011 |
| flow_concentration_10d_trend_z_scaled_std  |  0.0011 |   0.036 |             0.0001 |             0.0021 |

### Top 10 Notable Non-Robust Findings

| treatment_variable                      |   theta | p_value | is_robust | bias_phi | adj_conf_int_lower | adj_conf_int_upper | benchmark_r2_y | benchmark_r2_d |
|:-------|-------:|-------:|:-------|-------:|-------:|-------:|-------:|-------:|
| realized_volatility_trend_z_scaled_mean |  0.0056 |       0 | False     |    0.232 |            -0.2281 |             0.2392 |         0.0358 |         0.8459 |
| vix_trend_z_scaled_mean                 | -0.0071 |       0 | False     |   0.1721 |            -0.1811 |             0.1669 |         0.0439 |         0.8073 |
| vix_scaled_mean                         |  -0.023 |       0 | False     |   0.1539 |            -0.1869 |             0.1409 |         0.0439 |           0.79 |
| vix_scaled_last                         | -0.0015 |  0.0016 | False     |   0.1391 |            -0.1416 |             0.1386 |         0.0439 |         0.7833 |
| vix_trend_z_scaled_last                 | -0.0023 |  0.0001 | False     |    0.125 |            -0.1284 |             0.1239 |         0.0439 |         0.7594 |
| vix_roc63_scaled_last                   |  0.0021 |  0.0028 | False     |   0.1239 |            -0.1232 |             0.1274 |         0.0439 |         0.7484 |
| vix_roc63_scaled_trend                  |  0.0088 |  0.0005 | False     |    1.048 |            -1.0441 |             1.0618 |         0.0439 |         0.7161 |
| realized_volatility_scaled_last         | -0.0016 |  0.0013 | False     |   0.0925 |            -0.0951 |             0.0919 |         0.0358 |         0.7136 |
| upg_63d_scaled_mean                     |  0.0062 |       0 | False     |   0.1131 |            -0.1084 |             0.1207 |         0.0549 |         0.6981 |
| upg_63d_scaled_last                     |  0.0039 |       0 | False     |   0.0975 |            -0.0953 |             0.1032 |         0.0549 |         0.6785 |

## Comparative Analysis: DML-PLR vs. DML-APE

### Robustness Status Change Summary

-   **Total variables robust in PLR:** 27
-   **Total variables robust in APE:** 48
-   **Findings that remained robust:** 16
-   **Findings that LOST robustness (PLR -\> APE):** 11
-   **Findings that GAINED robustness (PLR -\> APE):** 32

### Variables that Remained Robust

| treatment_variable                         | theta_plr | theta_ape |
|:-------------------------------------------|----------:|----------:|
| ffr_slope_roc63_scaled_last                |   -0.0228 |   -0.0006 |
| fx_rv_6j_21d_trend_z_scaled_mean           |   -0.0143 |   -0.0017 |
| ffr_slope_scaled_last                      |   -0.0154 |    0.0177 |
| amihud_illiquidity_trend_z_scaled_std      |   -0.0608 |     0.016 |
| ffr_slope_scaled_mean                      |   -0.0145 |    0.0011 |
| fx_rv_6j_21d_trend_z_scaled_last           |   -0.0153 |   -0.0018 |
| ffr_slope_scaled_trend                     |   -0.1436 |   -0.0073 |
| pcr_oi_roc63_scaled_std                    |   -0.0549 |    0.0241 |
| flow_concentration_10d_scaled_std          |    0.0636 |    0.0021 |
| flow_concentration_10d_trend_z_scaled_mean |   -0.0093 |   -0.0013 |
| flow_concentration_10d_trend_z_scaled_std  |    0.0404 |    0.0011 |
| flow_concentration_10d_roc63_scaled_std    |    0.0515 |    0.0018 |
| ffr_basis_roc63_scaled_last                |    0.0081 |   -0.0003 |
| ffr_slope_trend_z_scaled_trend             |   -0.0834 |   -0.0066 |
| risk_neutral_kurtosis_scaled_mean          |    0.0173 |    0.0051 |
| pcr_oi_trend_z_scaled_std                  |   -0.0337 |    0.0213 |

### Variables that Lost Robustness

| treatment_variable                         | theta_plr | p_value_plr | benchmark_r2_d_plr |
|:----------------------------|--------------:|--------------:|--------------:|
| ffr_slope_trend_z_scaled_last              |   -0.0157 |           0 |                  0 |
| credit_spread_scaled_std                   |   -0.0524 |           0 |                  0 |
| credit_spread_trend_z_scaled_std           |   -0.0522 |           0 |                  0 |
| ffr_slope_roc63_scaled_mean                |   -0.0122 |      0.0001 |                  0 |
| fx_rv_6j_21d_scaled_mean                   |   -0.0128 |      0.0025 |             0.0069 |
| risk_neutral_skewness_scaled_trend         |   -0.1346 |      0.0069 |                  0 |
| risk_neutral_skewness_trend_z_scaled_trend |   -0.1533 |      0.0082 |                  0 |
| fx_rv_6j_21d_scaled_last                   |   -0.0096 |      0.0135 |                  0 |
| ffr_basis_roc63_scaled_mean                |    0.0111 |      0.0177 |                  0 |
| risk_neutral_kurtosis_trend_z_scaled_mean  |    0.0186 |      0.0196 |                  0 |
| risk_neutral_skewness_roc63_scaled_trend   |   -0.0946 |      0.0359 |                  0 |

### Variables that Gained Robustness

| treatment_variable                         | theta_ape | p_value_ape |
|:-------------------------------------------|----------:|------------:|
| risk_neutral_skewness_trend_z_scaled_std   |    0.0343 |           0 |
| vrp_roc63_scaled_std                       |   -0.0021 |      0.0099 |
| ffr_basis_roc63_scaled_trend               |    -0.002 |      0.0034 |
| fx_rv_6j_21d_roc63_scaled_std              |    0.0057 |           0 |
| risk_neutral_skewness_scaled_std           |    0.0359 |           0 |
| ffr_basis_scaled_mean                      |    0.0006 |      0.0345 |
| fx_momentum_6j_21d_trend_z_scaled_std      |    0.0026 |           0 |
| fx_momentum_6e_21d_trend_z_scaled_std      |    0.0047 |           0 |
| fx_momentum_6e_21d_scaled_std              |    0.0038 |           0 |
| ffr_slope_scaled_std                       |    0.0103 |           0 |
| ffr_basis_scaled_last                      |    0.0007 |      0.0096 |
| pcr_oi_scaled_std                          |    0.0191 |           0 |
| fx_rv_6j_21d_trend_z_scaled_std            |    0.0072 |           0 |
| risk_neutral_kurtosis_roc63_scaled_std     |    0.0382 |           0 |
| risk_neutral_kurtosis_trend_z_scaled_std   |    0.0485 |           0 |
| ffr_slope_roc63_scaled_std                 |    0.0063 |           0 |
| fx_rv_6j_21d_scaled_std                    |    0.0051 |           0 |
| risk_neutral_kurtosis_trend_z_scaled_trend |    -0.006 |      0.0233 |
| risk_neutral_skewness_roc63_scaled_std     |    0.0399 |           0 |
| gex_oi_trend_z_scaled_std                  |    0.0773 |           0 |
| fx_rv_6e_21d_roc63_scaled_mean             |   -0.0016 |           0 |
| fx_rv_6e_21d_trend_z_scaled_trend          |    0.0024 |      0.0009 |
| risk_neutral_kurtosis_scaled_std           |    0.0957 |           0 |
| fx_rv_6e_21d_trend_z_scaled_last           |   -0.0009 |           0 |
| fx_rv_6j_21d_trend_z_scaled_trend          |    0.0037 |           0 |
| fx_rv_6e_21d_roc63_scaled_std              |    0.0061 |           0 |
| risk_neutral_kurtosis_scaled_trend         |   -0.0043 |      0.0313 |
| fx_rv_6e_21d_roc63_scaled_last             |   -0.0012 |           0 |
| fx_rv_6e_21d_scaled_mean                   |   -0.0009 |      0.0003 |
| fx_rv_6e_21d_scaled_std                    |      0.01 |           0 |
| fx_rv_6e_21d_trend_z_scaled_mean           |   -0.0012 |           0 |
| ffr_slope_trend_z_scaled_std               |    0.0092 |           0 |

### Variables with Coefficient Sign Flips

| treatment_variable                         | theta_plr | is_robust_plr | theta_ape | is_robust_ape |
|:-----------------------|-----------:|:-----------|-----------:|:-----------|
| ffr_slope_scaled_last                      |   -0.0154 | True          |    0.0177 | True          |
| amihud_illiquidity_trend_z_scaled_std      |   -0.0608 | True          |     0.016 | True          |
| ffr_slope_scaled_mean                      |   -0.0145 | True          |    0.0011 | True          |
| pcr_oi_roc63_scaled_std                    |   -0.0549 | True          |    0.0241 | True          |
| risk_neutral_skewness_trend_z_scaled_trend |   -0.1533 | True          |    0.0013 | False         |
| ffr_basis_roc63_scaled_last                |    0.0081 | True          |   -0.0003 | True          |
| risk_neutral_skewness_roc63_scaled_trend   |   -0.0946 | True          |    0.0002 | False         |
| pcr_oi_trend_z_scaled_std                  |   -0.0337 | True          |    0.0213 | True          |
| fx_rv_6j_21d_roc63_scaled_std              |   -0.0321 | False         |    0.0057 | True          |
| ffr_basis_scaled_mean                      |   -0.0059 | False         |    0.0006 | True          |
| fx_momentum_6j_21d_trend_z_scaled_std      |   -0.0251 | False         |    0.0026 | True          |
| ffr_slope_scaled_std                       |   -0.0232 | False         |    0.0103 | True          |
| ffr_basis_scaled_last                      |   -0.0044 | False         |    0.0007 | True          |
| fx_rv_6j_21d_scaled_std                    |   -0.0139 | False         |    0.0051 | True          |
| risk_neutral_kurtosis_trend_z_scaled_trend |    0.0229 | False         |    -0.006 | True          |
| fx_rv_6e_21d_trend_z_scaled_trend          |   -0.0167 | False         |    0.0024 | True          |
| risk_neutral_kurtosis_scaled_std           |   -0.0055 | False         |    0.0957 | True          |
| fx_rv_6e_21d_trend_z_scaled_last           |    0.0021 | False         |   -0.0009 | True          |
| risk_neutral_kurtosis_scaled_trend         |    0.0124 | False         |   -0.0043 | True          |
| fx_rv_6e_21d_scaled_std                    |   -0.0024 | False         |      0.01 | True          |
| ffr_slope_trend_z_scaled_std               |   -0.0003 | False         |    0.0092 | True          |

### Special Case: Amihud Illiquidity Sign Reversal

As discussed, the effect of Amihud Illiquidity volatility reverses sign between the two models.

| treatment_variable                    | theta_plr | is_robust_plr | theta_ape | is_robust_ape |
|:---------------------|------------:|:------------|------------:|:------------|
| amihud_illiquidity_trend_z_scaled_std |   -0.0608 | True          |     0.016 | True          |
