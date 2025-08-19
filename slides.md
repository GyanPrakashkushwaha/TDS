---
marp: true
theme: default
paginate: true
backgroundImage: url('https://images.unsplash.com/photo-1551288049-bebda4e38f71?ixlib=rb-4.0.3&auto=format&fit=crop&w=1950&q=80')
style: |
  section {
    background-color: rgba(255, 255, 255, 0.9);
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  }
  h1 {
    color: #2c3e50;
    border-bottom: 3px solid #3498db;
    padding-bottom: 10px;
  }
  h2 {
    color: #34495e;
  }
  h3 {
    color: #7f8c8d;
  }
  strong {
    color: #e74c3c;
  }
  table {
    box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    border-radius: 8px;
  }
  blockquote {
    background: #ecf0f1;
    border-left: 4px solid #3498db;
    padding: 1rem;
    margin: 1rem 0;
  }
---

<!-- _backgroundImage: url('https://images.unsplash.com/photo-1557804506-669a67965ba0?ixlib=rb-4.0.3&auto=format&fit=crop&w=1974&q=80') -->
<!-- _color: white -->
<!-- _class: lead -->

# Q2 2025 Business Analysis
## Data-Driven Insights

### Technical Documentation & Analysis
**Presenter:** 23f3004091@ds.study.iitm.ac.in

---

<!-- _backgroundImage: url('https://images.unsplash.com/photo-1460925895917-afdab827c52f?ixlib=rb-4.0.3&auto=format&fit=crop&w=2015&q=80') -->
<!-- _class: invert -->

# Executive Summary

> **Performance Overview:** Q2 2025 delivered exceptional results across all key metrics

- **Revenue Growth**: 15% increase compared to Q1 2025
- **Market Expansion**: Entered 3 new regions
- **Customer Base**: 25% growth in active users
- **Profitability**: Improved margins by 8%

---

# Key Metrics Overview

| Metric | Q1 2025 | Q2 2025 | Change |
|--------|---------|---------|--------|
| Revenue | $2.1M | $2.4M | +15% |
| Users | 12,000 | 15,000 | +25% |
| Retention | 85% | 89% | +4% |
| Cost/User | $45 | $38 | -15% |

---

# Algorithm Performance Analysis

## Data Processing Complexity

Our analytics engine optimization results:

**Time Complexity Improvements:**
- Previous algorithm: $O(n^2 \log n)$
- New optimized version: $O(n \log n)$

**Space Complexity:**
- Memory usage: $O(n)$ where $n$ is dataset size

**Performance Metrics:**
$$\text{Efficiency Gain} = \frac{T_{old} - T_{new}}{T_{old}} \times 100\%$$

Where $T_{old} = 2.3s$ and $T_{new} = 0.8s$

$$\text{Efficiency Gain} = \frac{2.3 - 0.8}{2.3} \times 100\% = 65.2\%$$

---

# Market Performance

![bg right:40% 80%](https://via.placeholder.com/400x300/4CAF50/FFFFFF?text=Revenue+Growth+Chart)

- **Strong Q2 Performance**
- Exceeded targets by 12%
- Regional expansion successful
- Cost optimization effective

---

# Customer Insights

- **Demographics**: 60% millennials, 25% Gen Z
- **Geographic**: 40% urban, 35% suburban, 25% rural  
- **Engagement**: Average session time increased 18%
- **Satisfaction**: NPS score improved to 72

---

# Competitive Analysis

![bg left:30% 90%](https://via.placeholder.com/300x200/2196F3/FFFFFF?text=Market+Share)

### Our Position:
- Market share: 18% (up from 15%)
- 2nd largest in our segment
- Key differentiator: Customer service
- Competitive pricing advantage

---

# Financial Highlights

- **Gross Margin**: 68% (target: 65%)
- **Operating Expenses**: Reduced by 5%
- **Cash Flow**: Positive $890K
- **R&D Investment**: 12% of revenue

---

# Operational Efficiency

![bg right:35% 85%](https://via.placeholder.com/350x250/FF9800/FFFFFF?text=Efficiency+Metrics)

### Key Improvements:
- Process automation: 30% faster
- Error reduction: 25% decrease  
- Team productivity: Up 20%
- Customer response time: 40% faster

---

# Challenges & Risks

- **Supply Chain**: Minor delays in Q3
- **Competition**: New market entrants
- **Regulations**: Upcoming compliance changes
- **Talent**: Skills gap in tech roles

---

# Q3 2025 Outlook

### Priorities:
- Launch new product line
- Expand international presence  
- Strengthen supply chain partnerships
- Invest in team development

### Targets:
- Revenue: $2.8M (+17%)
- Users: 18,000 (+20%)

---

<!-- New Interactive Slide: Slider controls scenario projections -->
# Interactive Scenario — Revenue Projection

<!-- 
  Comment: This slide contains an interactive slider widget.
  Data flow:
   1. User moves the slider (input range) -> slider value (growthFactor) updates.
   2. JS calculates projected metrics using base values (from Q2 2025).
   3. JS updates DOM elements (these are the "dependent cells").
   4. Markdown-like outputs are rendered inside HTML containers so they update in real time.
-->

<div style="max-width:900px">
  <p><strong>Use the slider</strong> to simulate projected % growth multiplier for Q3 (from conservative to aggressive).</p>

  <!-- Slider input (controls the growth multiplier). This is the "source" cell. -->
  <label for="growthRange">Growth scenario: <span id="growthLabel">+15%</span></label>
  <input id="growthRange" type="range" min="0" max="40" value="17" step="1" style="width:100%;">

  <hr/>

  <!-- These are the dependent "cells" that update when slider changes. -->
  <div id="projectionOutputs" style="display:grid;grid-template-columns:1fr 1fr;gap:1rem;margin-top:1rem;">
    <div style="padding:1rem;border-radius:8px;box-shadow:0 2px 6px rgba(0,0,0,0.06);">
      <h3>Projected Revenue</h3>
      <div id="projRevenue" style="font-size:1.4rem;font-weight:700;">$2.8M</div>
      <div id="projRevenueNote" style="font-size:0.9rem;color:#555;">(based on multiplier)</div>
    </div>

    <div style="padding:1rem;border-radius:8px;box-shadow:0 2px 6px rgba(0,0,0,0.06);">
      <h3>Projected Active Users</h3>
      <div id="projUsers" style="font-size:1.4rem;font-weight:700;">18,000</div>
      <div id="projUsersNote" style="font-size:0.9rem;color:#555;">(user growth scales with revenue)</div>
    </div>

    <div style="padding:1rem;border-radius:8px;box-shadow:0 2px 6px rgba(0,0,0,0.06);">
      <h3>Projected Profit Margin</h3>
      <div id="projMargin" style="font-size:1.4rem;font-weight:700;">70%</div>
      <div id="projMarginNote" style="font-size:0.9rem;color:#555;">(margins improve slightly with scale)</div>
    </div>

    <div style="padding:1rem;border-radius:8px;box-shadow:0 2px 6px rgba(0,0,0,0.06);">
      <h3>Scenario Summary</h3>
      <div id="scenarioSummary" style="font-size:0.95rem;color:#333;">
        Conservative to aggressive scenario shown here. Adjust slider for values.
      </div>
    </div>
  </div>
</div>

<!--
  Inline script: calculates projections from base Q2 values.
  - baseRevenue, baseUsers, baseMargin represent the "input dataset" (Q2 2025).
  - growthPct is read from slider and used to compute projected values.
  - All dependent DOM nodes are updated — these are the "cells with variable dependencies".
-->
<script>
(function() {
  // Base (Q2 2025) values - these are our baseline dataset inputs.
  const baseRevenue = 2.4;   // in millions
  const baseUsers = 15000;   // users
  const baseMargin = 0.68;   // 68%

  // DOM elements
  const range = document.getElementById('growthRange');
  const growthLabel = document.getElementById('growthLabel');
  const projRevenue = document.getElementById('projRevenue');
  const projUsers = document.getElementById('projUsers');
  const projMargin = document.getElementById('projMargin');
  const scenarioSummary = document.getElementById('scenarioSummary');

  // Helper for formatting numbers
  function formatMoney(millions) {
    return '$' + (millions.toFixed(2)) + 'M';
  }
  function formatUsers(n) {
    return n.toLocaleString();
  }

  // Update function (runs whenever slider changes)
  function updateProjections() {
    // Slider value is percent growth over base (e.g., 17 -> +17%)
    const growthPct = Number(range.value);
    growthLabel.textContent = (growthPct >= 0 ? '+' : '') + growthPct + '%';

    // Calculate projected values
    const revenueProjected = baseRevenue * (1 + growthPct / 100);
    // Assume user growth scales 0.9x of revenue growth percentally (example logic)
    const usersProjected = Math.round(baseUsers * (1 + (growthPct * 0.9) / 100));
    // Assume margin improves modestly with scale, up to +5 percentage points at +40% growth
    const marginImprovement = Math.min(0.05, (growthPct / 40) * 0.05);
    const marginProjected = Math.min(0.85, baseMargin + marginImprovement);

    // Update DOM (these are the dependent "cells")
    projRevenue.textContent = formatMoney(revenueProjected);
    projUsers.textContent = formatUsers(usersProjected);
    projMargin.textContent = Math.round(marginProjected * 100) + '%';

    // Dynamic summary (acts like dynamic markdown output)
    scenarioSummary.innerHTML = `
      <strong>Scenario:</strong> ${growthPct}% projected growth.<br/>
      <strong>Revenue:</strong> ${formatMoney(revenueProjected)} (vs base ${formatMoney(baseRevenue)})<br/>
      <strong>Users:</strong> ${formatUsers(usersProjected)} (scales at 0.9× growth)<br/>
      <strong>Margin:</strong> ${Math.round(marginProjected*100)}% (improved by ${Math.round(marginImprovement*100)} pts)
    `;
  }

  // Attach handler and initialize
  range.addEventListener('input', updateProjections);
  updateProjections();
})();
</script>

---

# Thank You
## Questions & Discussion

**Contact Information:**
- **Email:** 23f3004091@ds.study.iitm.ac.in
- **Analytics Dashboard:** company.com/analytics
- **Next Review:** October 15, 2025

---

<!-- _paginate: false -->
<!-- _class: invert -->

## Document Information

**Version Control:**
- Repository: quarterly-earnings-presentation
- Branch: main
- Last Updated: August 17, 2025

**Formats Available:**
- Markdown (source)
- HTML (web presentation)
- PDF (printable)
- PowerPoint (export)
