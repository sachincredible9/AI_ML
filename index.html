
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Linear Regression Performance Metrics — Data Science Reference</title>
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;600;700;800&family=IBM+Plex+Mono:ital,wght@0,300;0,400;0,500;1,400&family=DM+Sans:ital,wght@0,300;0,400;0,500;1,400&display=swap" rel="stylesheet">
<style>
:root {
  --bg: #0A0A0F;
  --bg2: #0E0E16;
  --bg3: #12121A;
  --surface: #16161F;
  --border: #1E1E2E;
  --border2: #2A2A3A;
  --text: #E8E0D5;
  --text2: #9A9AAA;
  --text3: #6A6A7A;
  --text4: #3A3A4A;
  --gold: #C8A87A;
  --gold2: #8A7A6A;
}

* { margin:0; padding:0; box-sizing:border-box; }

body {
  background: var(--bg);
  color: var(--text);
  font-family: 'DM Sans', system-ui, sans-serif;
  line-height: 1.6;
  min-height: 100vh;
}

/* ── HEADER ── */
.header {
  border-bottom: 1px solid var(--border);
  padding: 52px 40px 44px;
  background: linear-gradient(180deg,#0D0D1A 0%,var(--bg) 100%);
  position: relative;
  overflow: hidden;
}
.header::before {
  content:'';
  position:absolute;inset:0;
  background: radial-gradient(ellipse at 20% 50%,#1a0a3a18 0%,transparent 60%),
              radial-gradient(ellipse at 80% 20%,#0a2a1a18 0%,transparent 60%);
  pointer-events:none;
}
.header-inner { position:relative; max-width:1100px; margin:0 auto; }
.kicker {
  display:inline-block;
  background:#1A1A2E;
  border:1px solid #2A2A4A;
  border-radius:4px;
  padding:4px 12px;
  font-family:'IBM Plex Mono',monospace;
  font-size:10px;
  letter-spacing:3px;
  color:var(--text3);
  text-transform:uppercase;
  margin-bottom:20px;
}
.header h1 {
  font-family:'Syne',sans-serif;
  font-size:clamp(28px,5vw,54px);
  font-weight:800;
  line-height:1.1;
  letter-spacing:-1px;
  color:#F0EAE0;
  margin-bottom:14px;
}
.header h1 em { color:var(--gold2); font-style:italic; font-weight:400; }
.header p {
  color:var(--text3);
  font-size:15px;
  max-width:580px;
  line-height:1.7;
  margin-bottom:28px;
}
.stats { display:flex; gap:28px; flex-wrap:wrap; }
.stat { display:flex; align-items:baseline; gap:8px; }
.stat-n { font-size:28px; color:var(--gold); font-weight:300; font-family:'Syne',sans-serif; }
.stat-l { font-size:11px; color:var(--text4); letter-spacing:1px; text-transform:uppercase; }

/* ── MAIN ── */
.main { max-width:1100px; margin:0 auto; padding:40px; }

/* ── FILTERS ── */
.filters { display:flex; gap:8px; flex-wrap:wrap; margin-bottom:32px; }
.filter-btn {
  padding:8px 18px;
  border-radius:3px;
  border:1px solid var(--border2);
  background:transparent;
  color:var(--text3);
  font-size:13px;
  cursor:pointer;
  transition:all .2s;
  font-family:'DM Sans',sans-serif;
  letter-spacing:.3px;
}
.filter-btn:hover { border-color:var(--gold2); color:var(--text2); }
.filter-btn.active { border-color:var(--gold2); background:rgba(138,122,106,.12); color:var(--gold); }
.filter-count {
  margin-left:6px;
  background:var(--surface);
  border-radius:10px;
  padding:1px 6px;
  font-size:11px;
  color:var(--text4);
}

/* ── METRICS GRID ── */
.metrics-grid {
  display:grid;
  grid-template-columns:repeat(auto-fill,minmax(280px,1fr));
  gap:16px;
  margin-bottom:48px;
}
.metric-card {
  background:var(--bg2);
  border:1px solid var(--border);
  border-radius:6px;
  padding:20px;
  cursor:pointer;
  transition:all .2s;
  position:relative;
  overflow:hidden;
}
.metric-card:hover { border-color:var(--border2); background:var(--bg3); transform:translateY(-1px); }
.metric-card.active { background:var(--surface); }
.metric-card .accent-bar {
  position:absolute;
  top:0;left:0;
  width:3px;height:100%;
  opacity:.3;
  transition:opacity .2s;
}
.metric-card.active .accent-bar,
.metric-card:hover .accent-bar { opacity:1; }

.card-top { display:flex; justify-content:space-between; align-items:flex-start; margin-bottom:12px; }
.metric-name { font-family:'Syne',sans-serif; font-size:22px; font-weight:700; letter-spacing:-.5px; }
.metric-full { font-size:11px; color:var(--text3); letter-spacing:.5px; margin-top:2px; }
.verdict-badge {
  border-radius:3px;
  padding:3px 8px;
  font-size:10px;
  letter-spacing:.5px;
  white-space:nowrap;
  border:1px solid;
}
.card-desc { font-size:13px; color:var(--text2); line-height:1.55; margin-bottom:14px; }
.card-eq {
  background:#0A0A12;
  border-radius:4px;
  padding:8px 12px;
  font-family:'IBM Plex Mono',monospace;
  font-size:12px;
  border:1px solid;
  margin-bottom:12px;
}
.mini-bars { display:flex; align-items:flex-end; gap:3px; height:36px; }
.mini-bar { width:8px; border-radius:2px 2px 0 0; border:1px solid; opacity:.6; }

/* ── DETAIL PANEL ── */
.detail-panel {
  border-radius:8px;
  margin-bottom:48px;
  overflow:hidden;
  border:1px solid;
  animation:slideDown .3s ease;
}
@keyframes slideDown { from{opacity:0;transform:translateY(-8px)} to{opacity:1;transform:translateY(0)} }

.detail-header {
  padding:28px 32px;
  display:flex;
  justify-content:space-between;
  align-items:flex-start;
  flex-wrap:wrap;
  gap:16px;
}
.detail-title-row { display:flex; align-items:center; gap:14px; margin-bottom:8px; }
.detail-name { font-family:'Syne',sans-serif; font-size:36px; font-weight:700; }
.detail-full { font-size:16px; color:var(--text2); letter-spacing:.5px; }

.close-btn {
  background:transparent;
  border:1px solid var(--border2);
  border-radius:4px;
  color:var(--text3);
  padding:6px 14px;
  cursor:pointer;
  font-size:13px;
  font-family:'DM Sans',sans-serif;
  transition:all .2s;
}
.close-btn:hover { border-color:var(--text3); color:var(--text2); }

/* Tabs */
.tabs { display:flex; border-bottom:1px solid var(--border); padding-left:32px; }
.tab-btn {
  padding:14px 20px;
  background:transparent;
  border:none;
  border-bottom:2px solid transparent;
  color:var(--text3);
  font-size:13px;
  cursor:pointer;
  letter-spacing:.5px;
  font-family:'DM Sans',sans-serif;
  transition:all .2s;
}
.tab-btn:hover { color:var(--text2); }
.tab-btn.active { border-bottom-color:var(--active-color,#fff); color:var(--active-color,#fff); }

.tab-content { padding:32px; display:none; }
.tab-content.active { display:block; }

/* tab layouts */
.two-col { display:grid; grid-template-columns:1fr 1fr; gap:24px; }
@media(max-width:640px){ .two-col{ grid-template-columns:1fr; } }

.section-label {
  font-family:'IBM Plex Mono',monospace;
  font-size:11px;
  letter-spacing:2px;
  color:var(--gold);
  text-transform:uppercase;
  margin-bottom:12px;
  font-weight:400;
}
.detail-desc { color:var(--text2); line-height:1.75; }
.range-box {
  background:#0A0A12;
  border-radius:4px;
  padding:12px 16px;
  font-family:'IBM Plex Mono',monospace;
  font-size:13px;
  margin-top:8px;
}
.helps-box {
  border-radius:6px;
  padding:16px;
  margin-top:8px;
}
.helps-box p { color:#B0B0C0; line-height:1.7; font-size:14px; }

.eq-display {
  border-radius:8px;
  padding:32px;
  text-align:center;
  margin-bottom:24px;
}
.eq-formula {
  font-family:'IBM Plex Mono',monospace;
  font-size:clamp(14px,2.5vw,22px);
  letter-spacing:1px;
  line-height:1.8;
}
.eq-vars { display:grid; grid-template-columns:repeat(auto-fill,minmax(180px,1fr)); gap:10px; margin-top:8px; }
.eq-var {
  background:var(--bg2);
  border:1px solid var(--border2);
  border-radius:4px;
  padding:10px 14px;
  font-family:'IBM Plex Mono',monospace;
  font-size:12px;
  color:var(--text2);
}

.use-item { display:flex; gap:10px; align-items:flex-start; margin-bottom:10px; }
.use-arrow { margin-top:2px; flex-shrink:0; }
.use-text { color:var(--text2); font-size:14px; line-height:1.55; }

.data-box {
  border-radius:6px;
  padding:16px;
  font-size:14px;
  color:var(--text2);
  line-height:1.6;
  margin-top:8px;
}

.checklist { display:grid; grid-template-columns:repeat(auto-fill,minmax(280px,1fr)); gap:12px; }
.check-item {
  background:var(--bg2);
  border:1px solid var(--border);
  border-radius:6px;
  padding:14px 16px;
  display:flex;
  gap:12px;
  align-items:flex-start;
}
.check-num {
  width:22px;height:22px;
  border-radius:3px;
  display:flex;align-items:center;justify-content:center;
  font-family:'IBM Plex Mono',monospace;
  font-size:11px;
  flex-shrink:0;
  margin-top:1px;
  border:1px solid;
}
.check-text { font-size:13px; color:var(--text2); line-height:1.55; }

/* ── DECISION MATRIX ── */
.matrix-box {
  background:var(--bg2);
  border:1px solid var(--border);
  border-radius:8px;
  overflow:hidden;
  margin-bottom:48px;
}
.matrix-header {
  padding:24px 32px;
  border-bottom:1px solid var(--border);
  display:flex;align-items:center;gap:12px;
}
.matrix-header h2 { font-size:18px; font-weight:400; color:#E0D8CC; font-family:'Syne',sans-serif; }
.matrix-header p { font-size:12px; color:var(--text3); margin-top:4px; }
.matrix-table { width:100%; border-collapse:collapse; }
.matrix-table th {
  padding:12px 24px;
  text-align:left;
  font-family:'IBM Plex Mono',monospace;
  font-size:10px;
  letter-spacing:2px;
  color:var(--text3);
  text-transform:uppercase;
  font-weight:400;
  background:#0A0A12;
  border-bottom:1px solid var(--border);
}
.matrix-table td {
  padding:14px 24px;
  border-bottom:1px solid #16161E;
  vertical-align:middle;
}
.matrix-table tr:last-child td { border-bottom:none; }
.matrix-table tr:nth-child(even) td { background:#0A0A12; }
.scenario-cell { font-size:14px; color:#C8C0B8; font-style:italic; }
.tags { display:flex; gap:6px; flex-wrap:wrap; }
.tag {
  border-radius:3px;
  padding:2px 9px;
  font-size:11px;
  font-family:'IBM Plex Mono',monospace;
  letter-spacing:.3px;
  border:1px solid;
}
.tag-avoid { background:rgba(255,71,87,.13); border-color:rgba(255,71,87,.3); color:#FF6B6B; }

/* ── GOLDEN RULES ── */
.rules-box {
  background:var(--bg2);
  border:1px solid var(--border);
  border-radius:8px;
  padding:32px;
  margin-bottom:48px;
}
.rules-box h2 { font-size:18px; font-weight:400; color:#E0D8CC; margin-bottom:24px; font-family:'Syne',sans-serif; }
.rules-grid { display:grid; grid-template-columns:repeat(auto-fill,minmax(280px,1fr)); gap:16px; }
.rule-card {
  background:#0A0A12;
  border-radius:6px;
  padding:18px;
  border:1px solid;
  border-left-width:3px;
}
.rule-title { font-size:14px; font-weight:500; margin-bottom:8px; }
.rule-body { font-size:13px; color:var(--text3); line-height:1.6; }

/* ── FOOTER ── */
.footer {
  border-top:1px solid var(--border);
  padding-top:24px;
  margin-bottom:40px;
  display:flex;
  justify-content:space-between;
  align-items:center;
  flex-wrap:wrap;
  gap:12px;
}
.footer span { font-size:11px; color:var(--text4); letter-spacing:1px; }

/* scrollbar */
::-webkit-scrollbar { width:6px; height:6px; }
::-webkit-scrollbar-track { background:var(--bg); }
::-webkit-scrollbar-thumb { background:var(--border2); border-radius:3px; }
</style>
</head>
<body>

<!-- HEADER -->
<div class="header">
  <div class="header-inner">
    <div class="kicker">Data Scientist Reference Guide</div>
    <h1>Linear Regression<br><em>Performance Metrics</em></h1>
    <p>A complete reference for evaluating, comparing, and selecting the right regression metrics. Built for AI Engineers, Data Scientists, and ML Practitioners.</p>
    <div class="stats">
      <div class="stat"><span class="stat-n">12</span><span class="stat-l">Metrics Covered</span></div>
      <div class="stat"><span class="stat-n">6</span><span class="stat-l">Categories</span></div>
      <div class="stat"><span class="stat-n">8</span><span class="stat-l">Decision Scenarios</span></div>
    </div>
  </div>
</div>

<div class="main">

  <!-- FILTERS -->
  <div class="filters" id="filters"></div>

  <!-- METRICS GRID -->
  <div class="metrics-grid" id="metricsGrid"></div>

  <!-- DETAIL PANEL -->
  <div id="detailPanel" style="display:none;"></div>

  <!-- DECISION MATRIX -->
  <div class="matrix-box">
    <div class="matrix-header">
      <span style="font-size:20px">🎯</span>
      <div>
        <h2>Metric Decision Matrix</h2>
        <p>Quick reference: which metric to use for your scenario</p>
      </div>
    </div>
    <div style="overflow-x:auto">
      <table class="matrix-table" id="matrixTable"></table>
    </div>
  </div>

  <!-- GOLDEN RULES -->
  <div class="rules-box">
    <h2>⚡ Golden Rules for Model Evaluation</h2>
    <div class="rules-grid" id="rulesGrid"></div>
  </div>

  <!-- FOOTER -->
  <div class="footer">
    <span>LINEAR REGRESSION METRICS REFERENCE — DATA SCIENCE TOOLKIT</span>
    <span>Click any metric card to expand full documentation →</span>
  </div>

</div>

<script>
const metrics = [
  {
    id:"mae", name:"MAE", full:"Mean Absolute Error", category:"error", color:"#FF6B6B",
    verdict:"Most Interpretable", verdictColor:"#4ECDC4",
    description:"Measures the average magnitude of errors in predictions, without considering direction. It's the mean of absolute differences between predicted and actual values.",
    equation:"MAE = (1/n) × Σ|yᵢ - ŷᵢ|",
    equationParts:["n = number of samples","yᵢ = actual value","ŷᵢ = predicted value"],
    range:"[0, ∞) — lower is better",
    whenToUse:["When all errors should be weighted equally","When outliers shouldn't dominate the metric","When interpretability matters (same unit as target)","Business problems where under/over-prediction cost is equal"],
    dataType:"Continuous numerical targets; robust to outliers in evaluation",
    helps:"Shows average prediction deviation in original units. A MAE of 5 means predictions are off by 5 units on average.",
    checks:["Compare MAE against target mean — MAE/mean < 10% is typically good","Check if MAE is stable across different data splits","Compare train vs test MAE for overfitting signs","Ensure scale matches domain expectations"]
  },
  {
    id:"mse", name:"MSE", full:"Mean Squared Error", category:"error", color:"#FF8E53",
    verdict:"Penalizes Outliers", verdictColor:"#FF6B6B",
    description:"Measures the average squared difference between predicted and actual values. Squaring penalizes larger errors more heavily than smaller ones.",
    equation:"MSE = (1/n) × Σ(yᵢ - ŷᵢ)²",
    equationParts:["n = number of samples","yᵢ = actual value","ŷᵢ = predicted value"],
    range:"[0, ∞) — lower is better",
    whenToUse:["When large errors are particularly undesirable","As a loss function during model training","When mathematical convenience matters (differentiable)","Financial forecasting where big misses are very costly"],
    dataType:"Continuous targets; sensitive to outliers — be cautious with noisy data",
    helps:"Heavily penalizes large errors. If MSE is much larger than MAE², outliers or large errors exist in the model.",
    checks:["MSE >> MAE² signals outlier predictions","Always check RMSE (√MSE) for interpretability","Compare normalized MSE across different datasets","Monitor if MSE spikes on specific data segments"]
  },
  {
    id:"rmse", name:"RMSE", full:"Root Mean Squared Error", category:"error", color:"#C44FFF",
    verdict:"Gold Standard", verdictColor:"#C44FFF",
    description:"Square root of MSE, bringing the error metric back to the same unit as the target variable. Balances penalizing large errors while staying interpretable.",
    equation:"RMSE = √[(1/n) × Σ(yᵢ - ŷᵢ)²]",
    equationParts:["n = number of samples","yᵢ = actual value","ŷᵢ = predicted value"],
    range:"[0, ∞) — lower is better",
    whenToUse:["Standard metric for regression benchmarking","When large errors must be penalized more than small ones","When comparing models on the same dataset","Kaggle competitions and academic papers"],
    dataType:"Continuous numerical targets; most widely used general-purpose metric",
    helps:"If RMSE > MAE significantly, your model has prediction outliers. RMSE ≈ MAE means errors are uniformly distributed.",
    checks:["RMSE/MAE ratio — close to 1.0 means uniform errors","RMSE relative to std of target variable","Plot residuals to see if RMSE is inflated by specific regions","Test RMSE stability across k-fold cross-validation"]
  },
  {
    id:"r2", name:"R²", full:"Coefficient of Determination", category:"fit", color:"#4ECDC4",
    verdict:"Most Explained", verdictColor:"#4ECDC4",
    description:"Represents the proportion of variance in the dependent variable explained by the independent variables. Indicates how well the model fits compared to a baseline (mean) model.",
    equation:"R² = 1 − [Σ(yᵢ − ŷᵢ)² / Σ(yᵢ − ȳ)²]",
    equationParts:["yᵢ = actual value","ŷᵢ = predicted value","ȳ = mean of actual values"],
    range:"(-∞, 1] — closer to 1 is better; negative means worse than baseline",
    whenToUse:["Evaluating overall model fit quality","Comparing models on the same dataset","Explaining model performance to stakeholders","Baseline metric for any regression problem"],
    dataType:"Any continuous target; less meaningful for non-linear relationships",
    helps:"R²=0.85 means the model explains 85% of variance. R²<0 means predicting the mean is better than your model.",
    checks:["R² alone can be misleading — always check residual plots","High R² with bad residual patterns indicates model issues","R² increases with more features even if irrelevant — use Adjusted R²","Check train vs test R² gap for overfitting"]
  },
  {
    id:"adj_r2", name:"Adj. R²", full:"Adjusted R-Squared", category:"fit", color:"#45B7D1",
    verdict:"Feature Penalty", verdictColor:"#45B7D1",
    description:"A modified version of R² that adjusts for the number of predictors in the model. Penalizes adding unnecessary features that don't improve model performance.",
    equation:"Adj. R² = 1 − [(1−R²)(n−1) / (n−p−1)]",
    equationParts:["n = number of samples","p = number of predictors","R² = coefficient of determination"],
    range:"(-∞, 1] — use over R² when comparing models with different feature counts",
    whenToUse:["Comparing models with different numbers of features","Feature selection — penalizes irrelevant features","Multiple linear regression evaluation","When preventing overfitting via feature bloat"],
    dataType:"Multiple regression scenarios; requires knowing number of predictors",
    helps:"If Adj. R² drops when adding a feature, that feature hurts the model. Always prefer Adj. R² over R² for multi-feature models.",
    checks:["If R² increases but Adj. R² decreases — feature is noise","Large gap between R² and Adj. R² = too many weak features","Compare Adj. R² across nested models","Use with AIC/BIC for comprehensive model selection"]
  },
  {
    id:"mape", name:"MAPE", full:"Mean Absolute Percentage Error", category:"percentage", color:"#FFD93D",
    verdict:"Business Friendly", verdictColor:"#FFD93D",
    description:"Expresses error as a percentage of actual values. Makes error scale-independent, allowing comparison across datasets with different magnitudes.",
    equation:"MAPE = (100/n) × Σ|(yᵢ − ŷᵢ) / yᵢ|",
    equationParts:["n = number of samples","yᵢ = actual value","ŷᵢ = predicted value"],
    range:"[0%, ∞) — lower is better; <10% is excellent, <20% good",
    whenToUse:["Comparing models across different scales","Business reporting (% error is intuitive)","Demand forecasting and sales prediction","When relative error matters more than absolute error"],
    dataType:"NEVER use when actual values can be zero or near-zero (division by zero!)",
    helps:"MAPE=5% means predictions are 5% off on average. Easy to communicate to non-technical stakeholders.",
    checks:["Verify no zero or near-zero actual values exist","MAPE penalizes under-predictions more than over-predictions","Check if MAPE is skewed by small-value samples","Use sMAPE for symmetric treatment of over/under-prediction"]
  },
  {
    id:"smape", name:"sMAPE", full:"Symmetric Mean Absolute Percentage Error", category:"percentage", color:"#F7DC6F",
    verdict:"Symmetric Error", verdictColor:"#F7DC6F",
    description:"A symmetric version of MAPE that treats over-prediction and under-prediction equally. Bounded between 0% and 200%, avoiding the asymmetry problem of MAPE.",
    equation:"sMAPE = (100/n) × Σ[2|yᵢ−ŷᵢ| / (|yᵢ|+|ŷᵢ|)]",
    equationParts:["yᵢ = actual value","ŷᵢ = predicted value","n = number of samples"],
    range:"[0%, 200%] — lower is better; symmetric around 0",
    whenToUse:["When MAPE's asymmetry is a problem","When both actual and predicted values are non-zero","Time series forecasting (M4 competition standard)","When you need a bounded percentage metric"],
    dataType:"Positive non-zero actual and predicted values; handles near-zero better than MAPE",
    helps:"Treats a 50% overestimate the same as a 50% underestimate, unlike MAPE which is biased toward penalizing underestimates.",
    checks:["Still undefined when both actual AND predicted are zero","Compare with MAPE — large difference signals asymmetric errors","Use for M-competition style evaluations","Check distribution of per-sample errors for bias"]
  },
  {
    id:"rmsle", name:"RMSLE", full:"Root Mean Squared Log Error", category:"log", color:"#A8E6CF",
    verdict:"Skewed Data", verdictColor:"#A8E6CF",
    description:"Measures RMSE on log-transformed values. Penalizes under-predictions more than over-predictions and is robust to large-scale differences between predictions.",
    equation:"RMSLE = √[(1/n) × Σ(log(ŷᵢ+1) − log(yᵢ+1))²]",
    equationParts:["yᵢ = actual value","ŷᵢ = predicted value","+1 avoids log(0)"],
    range:"[0, ∞) — lower is better; works on log scale",
    whenToUse:["Target variable spans multiple orders of magnitude","Under-prediction is more costly than over-prediction","Predicting prices, populations, counts","Kaggle competitions with exponential targets"],
    dataType:"Positive targets only; ideal for right-skewed distributions",
    helps:"A RMSLE of 0.1 on log scale represents ~10% relative error. Equalizes importance across different magnitude ranges.",
    checks:["All predictions must be positive (add +1 guard)","Compare on original vs log-transformed scale","Check if log-transforming target before training helps RMSLE","Verify that under-prediction penalty is acceptable for domain"]
  },
  {
    id:"medae", name:"MedAE", full:"Median Absolute Error", category:"robust", color:"#FF9FF3",
    verdict:"Outlier Immune", verdictColor:"#FF9FF3",
    description:"Uses the median instead of mean to measure central tendency of errors. Extremely robust to outliers — a single bad prediction won't distort this metric.",
    equation:"MedAE = median(|y₁−ŷ₁|, |y₂−ŷ₂|, ..., |yₙ−ŷₙ|)",
    equationParts:["yᵢ = actual value","ŷᵢ = predicted value","median = 50th percentile"],
    range:"[0, ∞) — lower is better; most robust error metric",
    whenToUse:["Data with heavy outliers in predictions","When you want to ignore extreme cases","Evaluating typical model performance excluding edge cases","Real estate, salary prediction with extreme values"],
    dataType:"Any continuous target; best used alongside MAE to reveal outlier impact",
    helps:"If MedAE << MAE, outlier predictions exist. The gap between them reveals how many extreme errors are present.",
    checks:["MAE − MedAE gap reveals outlier influence","Large gap = model has systematic failures on some inputs","Check which samples cause the largest individual errors","Use with error percentile analysis (P90, P95, P99)"]
  },
  {
    id:"maxerr", name:"Max Error", full:"Maximum Residual Error", category:"robust", color:"#FF4757",
    verdict:"Worst Case", verdictColor:"#FF4757",
    description:"The worst-case error — the largest single prediction error across all samples. Critical in safety-critical applications where worst-case matters most.",
    equation:"MaxError = max(|yᵢ − ŷᵢ|) for all i",
    equationParts:["yᵢ = actual value","ŷᵢ = predicted value","max = maximum value"],
    range:"[0, ∞) — lower is better; critical for safety systems",
    whenToUse:["Safety-critical applications (medical, autonomous vehicles)","When no single prediction can exceed a threshold","SLA-bound predictions in production systems","Quality assurance and acceptance testing"],
    dataType:"Any regression; use when worst-case guarantees are needed",
    helps:"One sample with Max Error = 100 can be catastrophic even if RMSE looks good. Always check Max Error for risk assessment.",
    checks:["Identify and analyze which sample causes max error","Check if max error occurs on edge cases or distribution tails","Set acceptable thresholds before model deployment","Use P99 error as a softer alternative"]
  },
  {
    id:"evs", name:"EVS", full:"Explained Variance Score", category:"fit", color:"#70A1FF",
    verdict:"Bias Detector", verdictColor:"#70A1FF",
    description:"Measures how much of the variance in the target variable the model explains. Similar to R² but does not account for systematic bias in predictions.",
    equation:"EVS = 1 − [Var(y − ŷ) / Var(y)]",
    equationParts:["Var(y − ŷ) = variance of residuals","Var(y) = variance of actual values"],
    range:"(-∞, 1] — 1 is perfect; equals R² when no bias exists",
    whenToUse:["When you want to separate variance explanation from bias","Comparing EVS vs R² to detect systematic bias","Advanced model diagnostics","When model has a consistent over/under-prediction tendency"],
    dataType:"Continuous targets; most useful when compared directly against R²",
    helps:"If EVS > R², your model has systematic bias (constant offset). The gap reveals how much bias vs variance contributes to errors.",
    checks:["EVS > R² = model has systematic bias","EVS = R² = no bias, only random error","Plot residuals vs predicted values for bias patterns","Check mean of residuals — should be near zero"]
  },
  {
    id:"d2", name:"D²", full:"D² Score (Absolute / Tweedie)", category:"fit", color:"#B388FF",
    verdict:"Loss-Agnostic", verdictColor:"#B388FF",
    description:"A generalization of R² for non-squared loss functions. D² absolute uses MAE-based comparison; D² Tweedie is used for count/insurance-type data with Tweedie distributions.",
    equation:"D² = 1 − [L(y, ŷ) / L(y, ȳ)]",
    equationParts:["L = any loss function (e.g., MAE, Tweedie)","ȳ = mean of actuals"],
    range:"(-∞, 1] — 1 is perfect; analogous to R² for non-MSE losses",
    whenToUse:["When using non-squared loss functions","Insurance claim modeling (Tweedie distribution)","Count data or zero-inflated targets","When MAE-based fit assessment is needed"],
    dataType:"Specialized distributions; Tweedie for positive-valued, zero-heavy data",
    helps:"Provides an R²-like interpretability for non-standard loss functions. Tells what % of loss is explained vs a naive baseline.",
    checks:["Choose correct variant: absolute, Tweedie, or Poisson","Compare D² to R² — if very different, loss function matters","Check power parameter p for Tweedie variant","Validate baseline model choice is appropriate"]
  }
];

const categories = [
  {id:"all",label:"All Metrics"},
  {id:"error",label:"Error Metrics"},
  {id:"fit",label:"Fit Metrics"},
  {id:"percentage",label:"Percentage"},
  {id:"log",label:"Log Scale"},
  {id:"robust",label:"Robust"}
];

const decisionMatrix = [
  {scenario:"Quick business report", recommended:["MAE","MAPE"], avoid:["MSE","RMSLE"]},
  {scenario:"Outliers in data", recommended:["MedAE","MAE"], avoid:["MSE","RMSE"]},
  {scenario:"Comparing models (same dataset)", recommended:["RMSE","R²","Adj. R²"], avoid:["MAPE"]},
  {scenario:"Multi-scale comparison", recommended:["MAPE","sMAPE","R²"], avoid:["MAE","MSE"]},
  {scenario:"Right-skewed targets", recommended:["RMSLE","MedAE"], avoid:["MSE","RMSE"]},
  {scenario:"Feature selection", recommended:["Adj. R²"], avoid:["R²"]},
  {scenario:"Safety-critical system", recommended:["Max Error","MedAE","RMSE"], avoid:["R²"]},
  {scenario:"Insurance / Count data", recommended:["D²","RMSLE"], avoid:["R²","MAPE"]}
];

const goldenRules = [
  {rule:"Never use a single metric", detail:"Always pair an error metric (MAE/RMSE) with a fit metric (R²/Adj. R²) for a complete picture.", color:"#C44FFF"},
  {rule:"Check train vs test gap", detail:"A large gap between training and test metrics is a sign of overfitting — your model memorized data.", color:"#4ECDC4"},
  {rule:"Inspect residuals always", detail:"Even a good R² can hide patterns. Plot residuals vs predicted values to catch systematic errors.", color:"#FF6B6B"},
  {rule:"Know your outlier sensitivity", detail:"Use RMSE when large errors are critical. Use MedAE when outliers should be ignored.", color:"#FFD93D"},
  {rule:"Scale matters for errors", detail:"MAE of 5 on a [0–10] target is terrible. MAE of 5 on a [0–10,000] target is great. Always contextualize.", color:"#A8E6CF"},
  {rule:"Use Adj. R² with multiple features", detail:"R² always increases when adding features. Adj. R² penalizes irrelevant ones. Always prefer it for multi-feature models.", color:"#45B7D1"}
];

let activeCategory = "all";
let activeMetric = null;
let activeTab = "overview";

const barHeights = [0.3,0.7,0.5,0.9,0.4,0.75,0.6,0.85];

function hex(color,alpha){ return color+Math.round(alpha*255).toString(16).padStart(2,'0'); }

function miniBars(color){
  return barHeights.map(h=>`<div class="mini-bar" style="height:${Math.round(h*32)}px;background:${hex(color,0.5)};border-color:${hex(color,0.8)}"></div>`).join('');
}

function renderFilters(){
  const el = document.getElementById('filters');
  el.innerHTML = categories.map(c=>{
    const count = c.id==='all' ? metrics.length : metrics.filter(m=>m.category===c.id).length;
    return `<button class="filter-btn${activeCategory===c.id?' active':''}" onclick="setCategory('${c.id}')">${c.label}<span class="filter-count">${count}</span></button>`;
  }).join('');
}

function renderGrid(){
  const filtered = activeCategory==='all' ? metrics : metrics.filter(m=>m.category===activeCategory);
  const el = document.getElementById('metricsGrid');
  el.innerHTML = filtered.map(m=>`
    <div class="metric-card${activeMetric?.id===m.id?' active':''}" onclick="selectMetric('${m.id}')">
      <div class="accent-bar" style="background:${m.color}"></div>
      <div class="card-top">
        <div>
          <div class="metric-name" style="color:${m.color}">${m.name}</div>
          <div class="metric-full">${m.full}</div>
        </div>
        <div class="verdict-badge" style="color:${m.verdictColor};border-color:${hex(m.verdictColor,0.35)};background:${hex(m.verdictColor,0.1)}">${m.verdict}</div>
      </div>
      <p class="card-desc">${m.description.substring(0,90)}…</p>
      <div class="card-eq" style="color:${m.color};border-color:${hex(m.color,0.2)}">${m.equation}</div>
      <div class="mini-bars">${miniBars(m.color)}</div>
    </div>
  `).join('');
}

function renderDetail(m){
  const tabLabels = [{id:'overview',icon:'📊',label:'Overview'},{id:'equation',icon:'∑',label:'Equation'},{id:'usage',icon:'🎯',label:'When to Use'},{id:'checklist',icon:'✓',label:'Checklist'}];
  return `
    <div class="detail-panel" style="border-color:${hex(m.color,0.3)}">
      <div class="detail-header" style="background:linear-gradient(135deg,${hex(m.color,0.05)} 0%,transparent 60%);border-bottom:1px solid ${hex(m.color,0.12)}">
        <div>
          <div class="detail-title-row">
            <span class="detail-name" style="color:${m.color}">${m.name}</span>
            <div class="verdict-badge" style="color:${m.verdictColor};border-color:${hex(m.verdictColor,0.4)};background:${hex(m.verdictColor,0.12)}">${m.verdict}</div>
          </div>
          <div class="detail-full">${m.full}</div>
        </div>
        <button class="close-btn" onclick="closeDetail()">✕ Close</button>
      </div>
      <div class="tabs">
        ${tabLabels.map(t=>`<button class="tab-btn${activeTab===t.id?' active':''}" style="${activeTab===t.id?'--active-color:'+m.color:''};" onclick="setTab('${t.id}','${m.id}')">${t.icon} ${t.label}</button>`).join('')}
      </div>
      ${renderTab(m)}
    </div>`;
}

function renderTab(m){
  if(activeTab==='overview') return `
    <div class="tab-content active">
      <div class="two-col">
        <div>
          <div class="section-label">Description</div>
          <p class="detail-desc">${m.description}</p>
          <div class="section-label" style="margin-top:24px">Valid Range</div>
          <div class="range-box" style="color:${m.color};border:1px solid ${hex(m.color,0.25)}">${m.range}</div>
        </div>
        <div>
          <div class="section-label">How it Helps</div>
          <div class="helps-box" style="background:${hex(m.color,0.06)};border:1px solid ${hex(m.color,0.15)}">
            <p>${m.helps}</p>
          </div>
          <div class="section-label" style="margin-top:24px">Residual Pattern (Illustrative)</div>
          <div style="background:#0A0A12;border:1px solid var(--border);border-radius:4px;padding:12px 16px;display:flex;align-items:center;gap:12px;">
            <svg width="120" height="40" viewBox="0 0 120 40">
              <line x1="0" y1="20" x2="120" y2="20" stroke="${hex(m.color,0.25)}" stroke-width="1" stroke-dasharray="3,2"/>
              ${[[10,20],[22,8],[35,28],[50,5],[62,22],[75,12],[88,30],[100,8]].map(([x,y])=>`<circle cx="${x}" cy="${y}" r="3" fill="${m.color}" opacity="0.8"/>`).join('')}
            </svg>
            <span style="color:var(--text4);font-size:11px">Predicted vs Residuals</span>
          </div>
        </div>
      </div>
    </div>`;

  if(activeTab==='equation') return `
    <div class="tab-content active">
      <div class="eq-display" style="background:#06060C;border:1px solid ${hex(m.color,0.35)};border-radius:8px">
        <div class="eq-formula" style="color:${m.color}">${m.equation}</div>
      </div>
      <div class="section-label">Variable Definitions</div>
      <div class="eq-vars">${m.equationParts.map(p=>`<div class="eq-var">${p}</div>`).join('')}</div>
    </div>`;

  if(activeTab==='usage') return `
    <div class="tab-content active">
      <div class="two-col">
        <div>
          <div class="section-label">When to Use</div>
          ${m.whenToUse.map(item=>`<div class="use-item"><span class="use-arrow" style="color:${m.color}">→</span><span class="use-text">${item}</span></div>`).join('')}
        </div>
        <div>
          <div class="section-label">Data Requirements</div>
          <div class="data-box" style="background:var(--bg2);border:1px solid ${hex(m.color,0.25)}">${m.dataType}</div>
        </div>
      </div>
    </div>`;

  if(activeTab==='checklist') return `
    <div class="tab-content active">
      <div class="section-label">Performance Measurement Checklist</div>
      <div class="checklist">${m.checks.map((item,i)=>`
        <div class="check-item">
          <div class="check-num" style="color:${m.color};border-color:${hex(m.color,0.4)}">${i+1}</div>
          <div class="check-text">${item}</div>
        </div>`).join('')}</div>
    </div>`;
  return '';
}

function renderMatrix(){
  const el = document.getElementById('matrixTable');
  el.innerHTML = `
    <thead><tr>
      <th>Scenario</th><th>Recommended Metrics</th><th>Avoid</th>
    </tr></thead>
    <tbody>${decisionMatrix.map(row=>`
      <tr>
        <td class="scenario-cell">${row.scenario}</td>
        <td><div class="tags">${row.recommended.map(name=>{
          const m = metrics.find(mx=>mx.name===name||mx.name.replace('Adj. ','')===name);
          const color = m ? m.color : '#4ECDC4';
          return `<span class="tag" style="color:${color};border-color:${hex(color,0.35)};background:${hex(color,0.12)}">${name}</span>`;
        }).join('')}</div></td>
        <td><div class="tags">${row.avoid.map(name=>`<span class="tag tag-avoid">${name}</span>`).join('')}</div></td>
      </tr>`).join('')}
    </tbody>`;
}

function renderRules(){
  const el = document.getElementById('rulesGrid');
  el.innerHTML = goldenRules.map(r=>`
    <div class="rule-card" style="border-color:${hex(r.color,0.25)};border-left-color:${r.color}">
      <div class="rule-title" style="color:${r.color}">${r.rule}</div>
      <div class="rule-body">${r.detail}</div>
    </div>`).join('');
}

function setCategory(cat){
  activeCategory = cat;
  renderFilters();
  renderGrid();
}

function selectMetric(id){
  const m = metrics.find(x=>x.id===id);
  if(activeMetric?.id===id){ closeDetail(); return; }
  activeMetric = m;
  activeTab = 'overview';
  renderGrid();
  const panel = document.getElementById('detailPanel');
  panel.style.display='block';
  panel.innerHTML = renderDetail(m);
  setTimeout(()=>panel.scrollIntoView({behavior:'smooth',block:'start'}),50);
}

function closeDetail(){
  activeMetric = null;
  document.getElementById('detailPanel').style.display='none';
  renderGrid();
}

function setTab(tab, metricId){
  activeTab = tab;
  const m = metrics.find(x=>x.id===metricId);
  const panel = document.getElementById('detailPanel');
  panel.innerHTML = renderDetail(m);
}

// Init
renderFilters();
renderGrid();
renderMatrix();
renderRules();
</script>
</body>
</html>
