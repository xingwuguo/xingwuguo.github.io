<style> 
.cases-container {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  margin: 30px 0;
}

.case-card {
  flex: 1;
  min-width: 280px;
  padding: 30px 25px;
  border-radius: 12px;
  display: flex;
  flex-direction: column;
  background: #fff9f9; /* Standardized Crimson background tint */
  border: 1px solid rgba(0,0,0,0.06);
  box-shadow: 0 2px 8px rgba(0,0,0,0.04);
  text-decoration: none !important;
  color: #2c3e50 !important;
  transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
  position: relative;
  overflow: hidden;
  border-top: 5px solid crimson; /* Standardized Crimson Accent */
}

.case-card:hover {
  transform: translateY(-8px);
  box-shadow: 0 12px 24px rgba(0,0,0,0.08);
  border-color: crimson;
}

.case-badge {
  font-size: 0.75rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 1px;
  color: crimson;
  margin-bottom: 15px;
  display: inline-block;
  padding: 4px 12px;
  background: rgba(220, 20, 60, 0.08); /* Crimson tint */
  border-radius: 20px;
  align-self: flex-start;
}

.case-title {
  font-size: 1.15rem;
  font-weight: 600;
  line-height: 1.5;
  margin-bottom: 25px;
  flex-grow: 1;
}

.case-footer {
  display: flex;
  align-items: center;
  font-size: 0.9rem;
  font-weight: 500;
  color: crimson;
  margin-top: auto;
}

.case-icon {
  margin-right: 8px;
  display: flex;
  align-items: center;
}

.case-card::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 4px;
  background: crimson;
  opacity: 0;
  transition: opacity 0.3s ease;
}

.case-card:hover::after {
  opacity: 1;
}
</style>

<div class="cases-container">
    <a href="../assets/成功案例/成功案例1-镁合金徽章制作技术.pdf" class="case-card">
        <span class="case-badge">Case 01</span>
        <div class="case-title">Manufacturing technology of magnesium alloy badge</div>
        <div class="case-footer">
            <span class="case-icon">
                <svg viewBox="0 0 24 24" width="18" height="18" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line><polyline points="10 9 9 9 8 9"></polyline></svg>
            </span>
            View Project Details
        </div>
    </a>

    <a href="../assets/成功案例/成功案例2-镁合金管材内外壁氧化技术.pdf" class="case-card">
        <span class="case-badge">Case 02</span>
        <div class="case-title">Oxidation technology of inner and outer wall of magnesium alloy pipe</div>
        <div class="case-footer">
            <span class="case-icon">
                <svg viewBox="0 0 24 24" width="18" height="18" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line><polyline points="10 9 9 9 8 9"></polyline></svg>
            </span>
            View Project Details
        </div>
    </a>

    <a href="../assets/成功案例/成功案例3-镁合金舱体与气门室罩处理技术.pdf" class="case-card">
        <span class="case-badge">Case 03</span>
        <div class="case-title">Treatment technology of magnesium alloy cabin and valve cover</div>
        <div class="case-footer">
            <span class="case-icon">
                <svg viewBox="0 0 24 24" width="18" height="18" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line><polyline points="10 9 9 9 8 9"></polyline></svg>
            </span>
            View Project Details
        </div>
    </a>

    <a href="../assets/成功案例/成功案例4-镁合金高耐蚀耐磨阳极氧化涂层技术.pdf" class="case-card">
        <span class="case-badge">Case 04</span>
        <div class="case-title">High corrosion resistance and wear resistance anodic oxidation coating technology for magnesium alloy</div>
        <div class="case-footer">
            <span class="case-icon">
                <svg viewBox="0 0 24 24" width="18" height="18" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path><polyline points="14 2 14 8 20 8"></polyline><line x1="16" y1="13" x2="8" y2="13"></line><line x1="16" y1="17" x2="8" y2="17"></line><polyline points="10 9 9 9 8 9"></polyline></svg>
            </span>
            View Project Details
        </div>
    </a>
</div>
