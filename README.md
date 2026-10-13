<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>English Tenses Revision</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="quiz-container">
    <header>
      <h1>English Tenses Revision</h1>
      <p>Test and refine your grammar knowledge</p>
    </header>

    <!-- Filter Section -->
    <div class="filter-section">
      <label for="tense-filter">Select Tense:</label>
      <select id="tense-filter">
        <option value="all">All Tenses</option>
        <option value="Present Simple">Present Simple</option>
        <option value="Present Continuous">Present Continuous</option>
        <option value="Past Simple">Past Simple</option>
        <option value="Present Perfect">Present Perfect</option>
      </select>
    </div>

    <!-- Progress Bar -->
    <div class="progress-bar-container">
      <div id="progress-bar"></div>
    </div>

    <!-- Question Card -->
    <div id="quiz-card" class="card">
      <div class="card-header">
        <span id="tense-badge" class="badge">Tense Category</span>
        <span id="score-tracker">Score: 0</span>
      </div>
      
      <p id="sentence-prompt" class="prompt">Loading sentence...</p>

      <div class="input-group">
        <input type="text" id="answer-input" placeholder="Type verb form here..." autocomplete="off">
        <button id="submit-btn">Check</button>
      </div>

      <div id="feedback" class="feedback hidden"></div>

      <button id="next-btn" class="next-btn hidden">Next Question →</button>
    </div>

    <!-- Completion View -->
    <div id="results-card" class="card hidden">
      <h2>Revision Complete! 🎉</h2>
      <p id="final-score">You scored 0 out of 0.</p>
      <button id="restart-btn">Try Again</button>
    </div>
  </div>

  <script src="app.js"></script>
</body>
</html>
