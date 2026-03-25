<h1>💰 Budget App – Full Stack Finance Manager</h1>
<p>A full-stack application for managing personal and group finances, built with Spring Boot (GraphQL) and React (Vite + TypeScript).</p>
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
<code>query {
  transactions {
    id
    amount
    type
  }
}
</code>
<h4>Example Mutation</h4>
<code>mutation {
  addTransaction(transactionDTO: {
    amount: 100
    type: "EXPENSE"
    tags: "food"
  }) {
    id
  }
}
</code>
<h2>📐 Data Model</h2>
<p align="center"><img src="https://i.imgur.com/J3ubXQM.png" alt="erd-diragram" width="80%"/></p>
<h2>▶️ Getting Started</h2>
<h4>1. Clone repository</h4>
<code>git clone https://github.com/karolklimonczykk/budget-app.git</code><br>
<code>cd budget-app</code>
<h4>2. Run database (Docker)</h4>
<code>docker compose up -d</code>
<h4>3. Run backend</h4>
<code>cd Backend</code><br>
<span>Using Maven:</span><code>./mvnw spring-boot:run</code><span>, or directly in IntelliJ.</span>
<h4>4. Run frontend</h4>
<code>cd Frontend</code><br>
<code>npm ci</code><br>
<code>npm run dev</code>
<h2>📸 Screenshots</h2>
<p align="center"><img src="https://i.imgur.com/tUKvws5.png" /></p>
<p align="center"><img src="https://i.imgur.com/ab4GCtN.png" /></p>
<p align="center"><img src="https://i.imgur.com/5dfwrmO.png" /></p>
<p align="center"><img src="https://i.imgur.com/cf4Xm7o.png" /></p>
<p align="center"><img src="https://i.imgur.com/EjLpydy.png"/></p>
<p align="center"><img src="https://i.imgur.com/CUGqvbM.png"/></p>
<p align="center"><img src="https://i.imgur.com/EpiIMQG.png"/></p>
<p align="center"><img src="https://i.imgur.com/i1OLLAe.png"/></p>
<p align="center"><img src="https://i.imgur.com/2lfPyF2.png"/></p>
<p align="center"><img src="https://i.imgur.com/o3A1WfQ.png"/></p>
<p align="center">Debt repayment for user <code>test2@test.pl</code></p>
<p align="center"><img src="https://i.imgur.com/Zs3uMDa.png"/></p>
<p align="center">Payment confirmation - user view <code>test@test.pl</code></p>
<p align="center"><img src="https://i.imgur.com/nF4r51z.png"/></p>
<p align="center"><img src="https://i.imgur.com/33yaF5C.png"/></p>
<p align="center">Payment confirmation - user view <code>test2@test.pl</code></p>
<p align="center"><img src="https://i.imgur.com/vgU0enB.png"/></p>
<p align="center">user <code>test@test.pl</code> transaction list:</p>
<p align="center"><img src="https://i.imgur.com/RKfUmQr.png"/></p>
<p align="center">user <code>test2@test.pl</code> transaction list:</p>
<p align="center"><img src="https://i.imgur.com/90y34Xt.png"/></p>
