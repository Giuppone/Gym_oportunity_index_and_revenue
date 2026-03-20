<h1>🏋️ Gym Opportunity Index & Revenue Model</h1>

<p>
A geospatial analytics project that identifies optimal locations for gym expansion using 
population data, competition density, and revenue estimation models.
</p>

<hr>

<h2>📍 Project Overview</h2>

<p>
This project transforms raw geospatial and demographic data into actionable business insights.
Using H3 hexagonal indexing, it evaluates where demand exceeds supply and estimates the 
potential revenue of opening a new gym.
</p>

<ul>
<li>Normalize geographic space using <b>H3 indexing</b></li>
<li>Estimate <b>demand</b> from population (ages 18–40)</li>
<li>Measure <b>competition</b from existing gyms</li>
<li>Compute an <b>Opportunity Index</b></li>
<li>Estimate <b>expected annual revenue</b> per zone</li>
</ul>

<hr>

<h2>🧠 Core Concepts</h2>

<h3>Opportunity Index</h3>
<p>
Measures imbalance between demand and supply:
</p>

<pre>
Opportunity ≈ Population / (Gyms + 1)
</pre>

<p>
A refined version prioritizes dense and underserved areas:
</p>

<pre>
Opportunity v2 ≈ (Population / (Gyms + 1)) * log(Population)
</pre>

---

<h3>Revenue Model</h3>

<pre>
Revenue ≈ Population × Penetration × Capture Rate × ARPU
</pre>

<ul>
<li><b>Penetration</b>: % of population likely to join a gym</li>
<li><b>Capture Rate</b>: market share vs competitors</li>
<li><b>ARPU</b>: average monthly revenue per user</li>
</ul>

<hr>

<h2>🗺️ Outputs</h2>

<ul>
<li>Hex-level demand vs competition maps</li>
<li>Opportunity heatmaps</li>
<li>Clustered expansion zones</li>
<li>Revenue estimation per zone</li>
</ul>

<p>
Interactive maps are built with <b>Folium</b> and can be deployed using <b>Streamlit</b>.
</p>

<hr>

<h2>⚙️ Tech Stack</h2>

<ul>
<li>Python (GeoPandas, Pandas, NumPy)</li>
<li>H3 (spatial indexing)</li>
<li>Folium (interactive maps)</li>
<li>Streamlit (deployment)</li>
</ul>

<hr>

<h2>🚀 Use Cases</h2>

<ul>
<li>Retail site selection</li>
<li>Franchise expansion strategy</li>
<li>Urban demand analysis</li>
<li>Location intelligence for physical businesses</li>
</ul>

<hr>

<h2>📊 Key Insight</h2>

<p>
Raw maps can be misleading due to geographic distortion. 
By normalizing space and combining demand with competition, 
we move from visualization to decision-making.
</p>

<hr>

<h2>🔜 Next Steps</h2>

<ul>
<li>Add income and socioeconomic layers</li>
<li>Incorporate distance-based competition</li>
<li>Optimize location selection under budget constraints</li>
<li>Deploy as an interactive decision dashboard</li>
</ul>

<hr>

<p><i>Built for data-driven location strategy and spatial intelligence.</i></p>
