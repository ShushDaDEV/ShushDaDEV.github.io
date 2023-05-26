# Purchase Coconut
## by TechHog

<!DOCTYPE html>
<html>
<head>
</head>
<body>
  <h1>Coconut</h1>

  <section>
    <h2>Code Snippet</h2>
    <pre><code>print("Hello")</code></pre>
    <button onclick="copyCode()">Copy</button>
  </section>

  <script>
    function copyCode() {
      const codeElement = document.querySelector('code');
      const codeText = codeElement.innerText;

      navigator.clipboard.writeText(codeText)
        .then(() => {
          alert('Code copied to clipboard!');
        })
        .catch((err) => {
          console.error('Failed to copy code: ', err);
        });
    }
  </script>
</body>
</html>
