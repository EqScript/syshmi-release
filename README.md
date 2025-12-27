# syshmi-core Distribution

This repository is used **only for binary releases** of `syshmi-core`.  
Source code is kept private — this repo exists to provide reproducible, versioned artifacts for the updater fleet.

---

## Workflow

1. **Build the binary**  
   The core application (`syshmi-core`) is compiled in a private environment.

2. **Bundle with manifest**  
   The binary and its `manifest.toml` are packaged together into a `.tar.gz` archive:
   ```bash
   tar -czvf syshmi-core-v0.0.1a.tar.gz syshmi-core manifest.toml

