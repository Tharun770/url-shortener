# url-shortener
A lightweight Flask-based URL Shortener API that converts long URLs into 6-character codes. Supports redirection, analytics (clicks, timestamp), and input validation. Uses in-memory storage with clean architecture, error handling, and test coverage using pytest. Fast, simple, and ideal for learning RESTful APIs.
<h2>📄 Project Description – Flask URL Shortener</h2>

<p>
This project is a lightweight yet functional <strong>URL Shortener API</strong>, similar in behavior to popular tools like Bitly and TinyURL.
Built using the <strong>Flask</strong> microframework, it offers an API-first design that allows users to convert long URLs into short, 6-character alphanumeric codes.
These shortened URLs can be used to quickly redirect to the original URL and are accompanied by basic analytics like click count and creation timestamps.
</p>

<p>
The main objective of this application is to demonstrate a complete feature implementation in Python using clean, maintainable code practices.
It handles routing, URL validation, code generation, analytics tracking, and error handling — all in an <strong>in-memory environment</strong>,
without relying on external databases. This makes the project easy to test, extend, and deploy for learning, demos, or lightweight production use cases.
</p>

<h3>🔧 Core Features:</h3>
<ul>
  <li><code>POST /api/shorten</code> – Accepts a long URL and returns a shortened version with a unique code.</li>
  <li><code>GET /&lt;short_code&gt;</code> – Redirects to the original URL, while incrementing the click count.</li>
  <li><code>GET /api/stats/&lt;short_code&gt;</code> – Returns analytics such as total clicks, creation time, and original URL.</li>
</ul>

<h3>🔍 Technical Highlights:</h3>
<ul>
  <li>URL validation to prevent invalid or harmful inputs.</li>
  <li>Thread-safe in-memory storage using Python dictionaries.</li>
  <li>Random short code generation (6 characters) ensuring uniqueness.</li>
  <li>Flask test client with pytest for automated unit testing.</li>
  <li>Error handling for 404 (not found) and 400 (bad request).</li>
  <li>Fully contained within a virtual environment with dependencies in <code>requirements.txt</code>.</li>
</ul>

<h3>📁 Structure:</h3>
<ul>
  <li><strong>main.py</strong> – Flask routes and API logic</li>
  <li><strong>models.py</strong> – In-memory database logic</li>
  <li><strong>utils.py</strong> – Helper functions (validation, code generation)</li>
  <li><strong>test_basic.py</strong> – Pytest-based unit tests</li>
  <li><strong>README.md</strong>, <strong>NOTES.md</strong>, and <strong>IMPLEMENTATION.md</strong> – Project documentation</li>
</ul>

<p>
This project is ideal for learners looking to practice Python APIs, Flask routing, test-driven development, or deploy microservices with lightweight architecture.
It adheres to clean code principles and separates concerns to encourage maintainable and scalable design.
</p>

