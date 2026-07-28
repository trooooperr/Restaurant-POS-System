<div>

<h1>Club POS System (V2.1 — Production Grade Hospitality ERP)</h1>

<p>
A <b>premium, production-ready Club POS & Management System</b> designed for modern hospitality businesses.
Engineered with <b>enterprise-level architecture, atomic data integrity, and modern UI/UX</b>, this system goes beyond a traditional POS and delivers a <b>full-scale hospitality ERP solution</b>.
</p>

<hr/>

<p align="center">
  <img src="https://github.com/user-attachments/assets/1594da58-5a05-4d37-9dbd-b36255a9597a" width="45%" />
  <img src="https://github.com/user-attachments/assets/13e80c05-75ef-442a-8c5d-aadaabde5a87" width="45%" />
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/f61f5527-2164-4af4-90c0-4caca78f3c43" width="45%" />
  <img src="https://github.com/user-attachments/assets/6640c4b4-7817-4cee-bb2e-3f0b77f40d16" width="45%" />
</p>

<h2>System Overview</h2>

<p>
The system follows a modular architecture with high-performance billing, secure role-based access, and real-time synchronization, making it suitable for busy club and hospitality environments.
</p>

<hr/>

<h2>Core Architecture (Separation of Concerns)</h2>

<h3>Kitchen Menu (Food Service Layer)</h3>

<ul>
<li>Managed through a dedicated <b>Menu Collection</b></li>
<li>Supports food-only items</li>
<li>No inventory dependency for faster billing</li>
</ul>

<h3>Beverage Inventory (Stock Layer)</h3>

<ul>
<li>Managed through a dedicated <b>Inventory Collection</b></li>
<li>Real-time inventory tracking</li>
<li>Automatic stock deduction after every order</li>
</ul>

<h3>Unified Billing Engine</h3>

<ul>
<li>Dynamically combines menu and inventory items</li>
<li>Supports multi-category billing</li>
<li>Optimized for low-latency operations</li>
</ul>

<hr/>

<h2>Premium UI/UX</h2>

<ul>
<li>Modern Glassmorphism interface</li>
<li>Responsive product grid with image previews</li>
<li>Smooth hover animations</li>
<li>Light & Dark themes</li>
<li>Desktop, tablet, and mobile optimized</li>
</ul>

<hr/>

<h2>Key Production Features</h2>

<ul>
<li><b>Atomic Bill Numbering:</b> Redis INCR prevents duplicate bill numbers</li>
<li><b>Inventory Management:</b> MongoDB bulkWrite ensures atomic stock updates</li>
<li><b>QR Ordering System:</b> Customers scan QR codes, browse menus, and place orders directly from their devices</li>
<li><b>Real-Time Synchronization:</b> Customer orders instantly appear on the POS dashboard</li>
<li><b>Silent Thermal Printing:</b> Automatic printing of KOTs and invoices</li>
<li><b>System Resilience:</b> In-memory database fallback</li>
<li><b>Scheduled Automation:</b> Node-Cron background jobs</li>
<li><b>Image-Based Menu:</b> Product image support for better usability</li>
</ul>

<hr/>

<h2>Security & Role Management</h2>

<table>
<tr>
<th>Role</th>
<th>Level</th>
<th>Access</th>
</tr>

<tr>
<td>Admin</td>
<td>L3</td>
<td>Full System Access</td>
</tr>

<tr>
<td>Manager</td>
<td>L2</td>
<td>Operations & Reporting</td>
</tr>

<tr>
<td>Staff</td>
<td>L1</td>
<td>Billing & Order Management</td>
</tr>

</table>

<ul>
<li>JWT Authentication</li>
<li>Role-Based Access Control (RBAC)</li>
<li>Password Recovery via OTP</li>
</ul>

<hr/>

<h2>E2E & Performance Testing</h2>

<p>
Comprehensive End-to-End testing and stress testing were performed to validate production readiness.
</p>

<table width="100%">

<tr>
<th align="left">Test</th>
<th align="left">Status</th>
<th align="left">Description</th>
</tr>

<tr>
<td><b>Complete Order Flow</b></td>
<td>PASS</td>
<td>Order → Billing → Settlement → Inventory Update</td>
</tr>

<tr>
<td><b>Authentication & RBAC</b></td>
<td>PASS</td>
<td>Verified permission-based access control</td>
</tr>

<tr>
<td><b>Inventory Consistency</b></td>
<td>PASS</td>
<td>No stock mismatch during concurrent billing</td>
</tr>

<tr>
<td><b>Atomic Operations</b></td>
<td>PASS</td>
<td>Verified Redis and MongoDB transactional workflows</td>
</tr>

<tr>
<td><b>Stress Test</b></td>
<td>PASS</td>
<td>Successfully processed 100+ parallel orders</td>
</tr>

<tr>
<td><b>Load Test</b></td>
<td>PASS</td>
<td>Simulated 7,500 virtual users using Artillery</td>
</tr>

<tr>
<td><b>Latency</b></td>
<td>PASS</td>
<td>Maintained low response time under heavy load</td>
</tr>

<tr>
<td><b>UI Stability</b></td>
<td>PASS</td>
<td>Smooth performance during continuous billing operations</td>
</tr>

</table>

<p>
<b>Result:</b> Production-ready application with stable performance under real-world hospitality workloads.
</p>

<hr/>

<h2>Technology Stack</h2>

<ul>
<li><b>Frontend:</b> React 18, Vite</li>
<li><b>Backend:</b> Node.js, Express.js</li>
<li><b>Database:</b> MongoDB Atlas</li>
<li><b>Caching:</b> Upstash Redis</li>
<li><b>Testing:</b> Jest, Supertest, Artillery</li>
</ul>

<hr/>

<h2>Deployment</h2>

<pre>
npm run build
npm start
</pre>

<pre>
CLOUD_MONGO_URI=
UPSTASH_REDIS_REST_URL=
UPSTASH_REDIS_REST_TOKEN=
JWT_SECRET=
ADMIN_EMAIL=
VITE_API_URL=
</pre>

<hr/>

<h2>Local Development</h2>

<pre>
npm install
cp .env.example .env
npm run dev
</pre>

<hr/>

<h2>Highlights</h2>

<ul>
<li>Production-grade hospitality ERP architecture</li>
<li>High-performance billing engine</li>
<li>Real-time QR ordering workflow</li>
<li>Atomic inventory management</li>
<li>Enterprise-level RBAC security</li>
<li>Automated thermal printing</li>
<li>Responsive React-based UI</li>
<li>Designed for real-world hospitality operations</li>
</ul>

</div>
