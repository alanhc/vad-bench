# VAD Benchmark (GitHub Pages)

A single-file static site that benchmarks:
- WebRTC VAD (libfvad via WASM)
- Silero VAD (ONNX Runtime Web via `@ricky0123/vad-web`)
- Simple Energy baseline

## Deploy to GitHub Pages

1. Create a new GitHub repo (e.g. `vad-benchmark`)
2. Commit `index.html` and push to `main`
3. Go to **Settings → Pages**
4. Source: **Deploy from a branch**
5. Branch: `main`, Folder: `/ (root)`
6. Open the Pages URL

## How to use

- Upload an audio file
- (Optional) upload a ground-truth JSON: `[{"startMs":1200,"endMs":3100}, ...]`
- Click **Run benchmark**
- Click **Export JSON** to copy/save results

## Notes

- Microphone permission is not required (offline file mode).
- Uses CDN dependencies; the page must be served over https (GitHub Pages is fine).
