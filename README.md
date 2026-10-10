# skimmer apt repository

Signed Debian packages for [skimmer](https://github.com/dorkitude/skimmer), published by its release workflow and served over GitHub Pages.

```bash
curl -fsSL https://dorkitude.github.io/skimmer-apt/key.gpg | sudo gpg --dearmor -o /usr/share/keyrings/skimmer.gpg
echo "deb [signed-by=/usr/share/keyrings/skimmer.gpg] https://dorkitude.github.io/skimmer-apt stable main" | sudo tee /etc/apt/sources.list.d/skimmer.list
sudo apt update && sudo apt install skimmer
```
