<div align="center">

# 🏛 CivicSense

### 🚀 Production-Grade Civic Engagement & Urban Transparency Platform

<img src="https://img.shields.io/badge/Status-Active-00C853?style=for-the-badge" />
<img src="https://img.shields.io/badge/Backend-Node.js-1E1E1E?style=for-the-badge&logo=node.js" />
<img src="https://img.shields.io/badge/Frontend-React-1E1E1E?style=for-the-badge&logo=react" />
<img src="https://img.shields.io/badge/Database-PostgreSQL-1E1E1E?style=for-the-badge&logo=postgresql" />
<img src="https://img.shields.io/badge/Cache-Redis-1E1E1E?style=for-the-badge&logo=redis" />
<img src="https://img.shields.io/badge/Containerized-Docker-1E1E1E?style=for-the-badge&logo=docker" />
<img src="https://img.shields.io/badge/CI/CD-GitHub%20Actions-1E1E1E?style=for-the-badge&logo=githubactions" />
<img src="https://img.shields.io/badge/Payments-Razorpay-1E1E1E?style=for-the-badge" />
<img src="https://img.shields.io/badge/Email-SendGrid-1E1E1E?style=for-the-badge" />

<br><br>

<strong>Report. Participate. Improve.</strong>

</div>


<h2> Overview</h2>

<p>
<strong>CivicSense</strong> is a full-stack civic collaboration platform that enables citizens to:
</p>

<ul>
  <li> Report public infrastructure issues with geolocation</li>
  <li> Submit and vote on civic improvement proposals</li>
  <li> Earn rewards for meaningful civic participation</li>
  <li> Track transparency metrics and analytics</li>
  <li> Receive verified public alerts</li>
  <li> Participate in community events</li>
  <li> Support the platform through donations</li>
</ul>

<p>
Built with a production mindset, CivicSense integrates Redis caching, CI/CD pipelines, Docker containerization, background workers, email providers, and payment gateways.
</p>

<hr>

<h2> Core Features</h2>

<h3> Issue Reporting</h3>
<ul>
  <li>Image upload with EXIF geolocation extraction</li>
  <li>Interactive map location selection</li>
  <li>Reverse geocoding to fetch address</li>
  <li>Weather snapshot at report time</li>
  <li>Status tracking with full timeline history</li>
  <li>Upvotes and duplicate detection</li>
</ul>

<h3> Civic Proposals</h3>
<ul>
  <li>Submit improvement ideas</li>
  <li>Community voting system</li>
  <li>Automatic escalation when threshold reached</li>
</ul>

<h3> Rewards & Leaderboard</h3>
<ul>
  <li>Points for verified reports</li>
  <li>Bonus points for high-impact issues</li>
  <li>Event participation rewards</li>
  <li>Weekly / Monthly / All-time leaderboard</li>
  <li>Badge system (Bronze, Silver, Gold, Civic Guardian)</li>
</ul>

<h3> Transparency Dashboard</h3>
<ul>
  <li>Resolution trends</li>
  <li>Area-based performance metrics</li>
  <li>Category distribution</li>
  <li>Authority accountability insights</li>
</ul>

<h3> Alerts System</h3>
<ul>
  <li>Verified emergency alerts</li>
  <li>Mass notification capability</li>
</ul>

<h3> Civic Events</h3>
<ul>
  <li>Community clean-ups</li>
  <li>Volunteer programs</li>
  <li>RSVP tracking</li>
</ul>

<h3> Donation Integration</h3>
<ul>
  <li>Secure payments via Razorpay</li>
  <li>Webhook verification</li>
  <li>Email receipts</li>
  <li>Donation transparency display</li>
</ul>

<hr>

<h2> Tech Stack</h2>

<h3>Frontend</h3>
<ul>
  <li>React + Vite</li>
  <li>Tailwind CSS</li>
  <li>Axios</li>
  <li>Chart.js</li>
</ul>

<h3>Backend</h3>
<ul>
  <li>Node.js</li>
  <li>Express.js</li>
  <li>PostgreSQL</li>
  <li>Redis (Caching + Rate Limiting + Queue)</li>
</ul>

<h3>Infrastructure</h3>
<ul>
  <li>Docker & Docker Compose</li>
  <li>GitHub Actions (CI/CD)</li>
  <li>Cloudinary (Image Hosting)</li>
  <li>Razorpay (Payments)</li>
  <li>SendGrid (Email Service)</li>
</ul>

<hr>

<h2> Architecture Overview</h2>

<pre>
Client (React)
      ↓
Backend API (Express)
      ↓
PostgreSQL (Primary DB)
      ↓
Redis (Cache + Queue + Rate Limiting)
      ↓
Worker Service (Async Jobs)
      ↓
External APIs (Maps, Weather, Email, Payments)
</pre>

<hr>

<h2> Database Design</h2>

<ul>
  <li>Users</li>
  <li>Issues</li>
  <li>Status History</li>
  <li>Proposals</li>
  <li>Votes</li>
  <li>Events</li>
  <li>Attendance</li>
  <li>Points Log</li>
  <li>Donations</li>
  <li>Audit Logs</li>
</ul>

<p>
Uses relational modeling, foreign keys, indexing, aggregation queries, and window functions for leaderboard ranking.
</p>

<hr>

<h2> Performance Optimizations</h2>

<ul>
  <li>Redis caching for leaderboard & analytics</li>
  <li>Geospatial indexing</li>
  <li>Rate limiting to prevent spam</li>
  <li>Background job queue for emails & rewards</li>
  <li>Query optimization with indexed columns</li>
</ul>

<hr>

<h2> Security</h2>

<ul>
  <li>JWT Authentication</li>
  <li>Role-based access control</li>
  <li>Password hashing</li>
  <li>Webhook verification</li>
  <li>Environment-based configuration</li>
  <li>Input validation & sanitization</li>
</ul>

<hr>

<h2> Docker Setup</h2>

<p>Services included:</p>

<ul>
  <li>Frontend</li>
  <li>Backend</li>
  <li>PostgreSQL</li>
  <li>Redis</li>
  <li>Worker Service</li>
  <li>pgAdmin</li>
</ul>

<p>Run locally:</p>

<pre>
docker-compose up --build
</pre>

<hr>

<h2> CI/CD Pipeline</h2>

<p>Using GitHub Actions:</p>

<ul>
  <li>Dependency installation</li>
  <li>Linting</li>
  <li>Testing</li>
  <li>Docker image build</li>
  <li>Deployment trigger</li>
</ul>

<hr>

<h2> Future Enhancements</h2>

<ul>
  <li>Real-time notifications with WebSockets</li>
  <li>Mobile PWA support</li>
  <li>AI-based duplicate detection</li>
  <li>Authority performance scoring</li>
</ul>

<hr>

<h2> Why CivicSense?</h2>

<p>
CivicSense is not just a CRUD application.  
It demonstrates:
</p>

<ul>
  <li>Advanced relational database design</li>
  <li>Event-driven architecture</li>
  <li>Asynchronous processing</li>
  <li>Production-ready DevOps workflow</li>
  <li>Scalable system thinking</li>
</ul>

<hr>

<h2> Author</h2>

<p>
Built with full-stack engineering principles and production architecture mindset.
</p>

<hr>

<p align="center">
  <strong>Making civic engagement transparent, rewarding, and impactful.</strong>
</p>
