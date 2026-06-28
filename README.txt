PUBLISHING "TCOTF"
====================================

This folder is your whole book, ready for free static hosting (e.g. GitHub Pages).

WHAT'S INSIDE
  book.html        the reader — open it to read locally, or host it
  manifest.json    your text, cues, effects & settings (already embedded in book.html too)
  assets/audio/    1 audio file(s), consistently named
  assets/img/      2 image file(s), consistently named

TO PUBLISH ON GITHUB PAGES
  1. Create a repository (or open your existing one).
  2. Drag EVERYTHING in this folder into the repo root — keep the assets/ folder
     exactly as-is (book.html must sit NEXT TO the assets/ folder).
  3. Commit & push (or use GitHub's "Add file > Upload files" in the browser).
  4. Settings > Pages > deploy from your main branch. Your book is live at
     https://<you>.github.io/<repo>/book.html

HOW RETRIEVAL WORKS
  The reader fetches each track/illustration ONLY when the reader reaches it
  (lazy), by its stable path under assets/. Nothing loads up front, so audio
  bandwidth stays low and the first page opens instantly.

NOTE: reader comments & analytics need the optional Supabase step — see the
project spec. Without it, the book reads & plays perfectly; discussion is local-only.