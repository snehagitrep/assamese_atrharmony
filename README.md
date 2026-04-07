 (cd "$(git rev-parse --show-toplevel)" && git apply --3way <<'EOF' 
diff --git a/README.md b/README.md
index 79e41b2b5ced840d89d5e5d43f4cf58cfba425e6..41585b6f3941983615bf9a2434033a8654b07ece 100644
--- a/README.md
+++ b/README.md
@@ -1 +1,16 @@
-# assamese_atrharmony
\ No newline at end of file
+# assamese_atrharmony
+
+Simple browser-based demo page for:
+
+- Uploading and playing an audio file
+- Generating a spectrogram visualization from the audio
+- Estimating basic formant trajectories (F1/F2/F3) from spectral peaks
+- Uploading external spectrogram and formant-trajectory images for side-by-side viewing
+
+## Run locally
+
+```bash
+python3 -m http.server 8000
+```
+
+Then open <http://localhost:8000> in your browser.
 
EOF
)
