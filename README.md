<style>
html {
  scroll-behavior: smooth; /* Enables gentle scroll descent */
}

.ceremonial-nav {
  text-align: center;
  background: linear-gradient(to right, gold, orange);
  padding: 12px;
  border-radius: 8px;
  font-weight: bold;
  font-size: 1.1em;
  position: sticky; /* Keeps ribbon visible while scrolling */
  top: 0;
  z-index: 1000;
}

.ceremonial-nav a {
  color: white;
  text-decoration: none;
  margin: 0 10px;
  transition: text-shadow 0.3s, color 0.3s;
}

.ceremonial-nav a:hover {
  color: #fffacd;
  text-shadow: 0 0 8px gold;
}

.ceremonial-nav .divider {
  color: white;
  margin: 0 5px;
}
</style>
