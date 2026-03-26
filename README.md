![Java](https://img.shields.io/badge/backend-Java-orange)
![Spring Boot](https://img.shields.io/badge/framework-SpringBoot-green)
![React](https://img.shields.io/badge/frontend-React-blue)
![GraphQL](https://img.shields.io/badge/API-GraphQL-pink)
<h1>💰 Budget App – Full Stack Finance Manager</h1>

> Full-stack finance manager with group expenses, debt tracking, and real-time balance analysis.
<h2>🚀 Overview</h2>
<p>Budget App is a full-stack system that allows users to:
<ul>
<li>track personal income and expenses</li>
<li>manage shared finances in groups</li>
<li>create and settle debts between users</li>
<li>analyze financial balance</li>
</ul>
The project is structured as a monorepo with a clear separation between backend and frontend.</p>
<h2>🧠 Features</h2>
<h3>📊 Personal Finance</h3>
<ul>
<li>Add, update and delete transactions</li>
<li>Categorize transactions (tags, notes)</li>
<li>View balance summary for given period of time</li>
</ul>
<h3>👥 Group Management</h3>
<ul>
<li>Create and manage groups</li>
<li>Add and remove members</li>
<li>Track shared expenses/incomes</li>
  </ul>
<h3>💸 Debt System</h3>
  <ul>
<li>Create debts between users</li>
<li>Mark debts as paid</li>
<li>Confirm payments (debtor ↔ creditor flow)</li>
</ul>
<h2>🖥️ Tech Stack</h2>
<h3>🔙 Backend</h3>
<ul>
<li>Java</li>
<li>Spring Boot</li>
<li>GraphQL</li>
<li>Hibernate / JPA</li>
</ul>
<h3>🎨 Frontend</h3>
<ul>
<li>React (Vite + Typescript)</li>
<li>SCSS</li>
</ul>
<h3>🗄️ Database</h3>
<ul>
<li>MySQL</li>
</ul>
<h3>⚙️ DevOps / Tools / Environments used</h3>
<ul>
<li>Docker (database)</li>
<li>GitHub Actions (CI)</li>
<li>SonarQube (code quality analysis)</li>
<li>IntelliJ IDEA 2024.3.3</li>
<li>Visual Studio Code</li>
</ul>
<h2>🔌 API (GraphQL)</h2>
<p>The backend exposes a GraphQL API with queries and mutations.</p>
<h4>Example Query</h4>

```graphql
query {
  transactions {
    id
    amount
    type
  }
}
```

<h4>Example Mutation</h4>

```graphql
mutation {
  addTransaction(transactionDTO: {
    amount: 100
    type: "EXPENSE"
    tags: "food"
  }) {
    id
  }
}
```

<h2>📐 Data Model</h2>
<p align="center"><img src="https://i.imgur.com/J3ubXQM.png" alt="erd-diragram" width="80%"/></p>
<h2>▶️ Getting Started</h2>
<h4>1. Clone repository</h4>

```bash
git clone https://github.com/karolklimonczykk/budget-app.git
cd budget-app
```

<h4>2. Run database (Docker)</h4>

```bash
docker compose up -d
```

<h4>3. Run backend</h4>

```bash
cd Backend
```

<span>Using Maven:</span><code>./mvnw spring-boot:run</code><span>, or directly in IntelliJ.</span>
<h4>4. Run frontend</h4>

```bash
cd Frontend
npm ci
npm run dev
```

<h2>📸 Screenshots</h2>

### 📊 Dashboard

<p align="center"><img src="https://i.imgur.com/tUKvws5.png" /></p>
<p align="center"><img src="https://i.imgur.com/ab4GCtN.png" /></p>
<p align="center"><img src="https://i.imgur.com/5dfwrmO.png" /></p>

### 💸 Transactions

<p align="center"><img src="https://i.imgur.com/cf4Xm7o.png" /></p>
<p align="center"><img src="https://i.imgur.com/EjLpydy.png"/></p>
<p align="center"><img src="https://i.imgur.com/CUGqvbM.png"/></p>

### 👥 Groups

<p align="center"><img src="https://i.imgur.com/EpiIMQG.png"/></p>
<p align="center"><img src="https://i.imgur.com/i1OLLAe.png"/></p>

### 🔁 Debt Flow

<p align="center"><img src="https://i.imgur.com/2lfPyF2.png"/></p>
<p align="center"><img src="https://i.imgur.com/o3A1WfQ.png"/></p>
<p align="center"><b>Debt repayment for user <code>test2@test.pl</code></b></p>
<p align="center"><img src="https://i.imgur.com/Zs3uMDa.png"/></p>
<p align="center"><b>Payment confirmation - user view <code>test@test.pl</code></b></p>
<p align="center"><img src="https://i.imgur.com/nF4r51z.png"/></p>
<p align="center"><img src="https://i.imgur.com/33yaF5C.png"/></p>
<p align="center"><b>Payment confirmation - user view <code>test2@test.pl</code></b></p>
<p align="center"><img src="https://i.imgur.com/vgU0enB.png"/></p>
<p align="center"><b>user <code>test@test.pl</code> transaction list:</b></p>
<p align="center"><img src="https://i.imgur.com/RKfUmQr.png"/></p>
<p align="center"><b>user <code>test2@test.pl</code> transaction list:</b></p>
<p align="center"><img src="https://i.imgur.com/90y34Xt.png"/></p>
<h2>🎯 What This Project Demonstrates</h2>
<ul>
<li>Full-stack development (Java + React)</li>
<li>GraphQL API design</li>
<li>Clean backend architecture (layered approach)</li>
<li>Handling complex relationships (groups, debts)</li>
<li>Integration between frontend and backend</li>
<li>Working with Docker and CI pipelines</li>
</ul>
<h2>👤 Author</h2>
Karol Klimończyk

[GitHub](https://github.com/karolklimonczykk)
