PUBLISHING "The Covenant of the Flowers"
====================================

This folder is your whole book, ready for free static hosting (e.g. GitHub Pages).

WHAT'S INSIDE
  wardens          the reader — open it to read locally, or host it
  manifest.json    your text, cues, effects & settings (already embedded in book.html too)
  assets/audio/    13 audio file(s), consistently named
  assets/img/      9 image file(s), consistently named

TO PUBLISH ON GITHUB PAGES (in the browser)
  1. In your repo, click "Add file" > "Upload files".
  2. Drag wardens, manifest.json and README.txt onto the page.
  3. THEN drag the WHOLE "assets" folder onto the SAME page (drop it on the
     "Drag additional files here" box). GitHub keeps the assets/audio and
     assets/img folders intact, and lists the files inside as assets/...
     !! IMPORTANT: the blue "choose your files" link CANNOT pick a folder --
     it only takes single files. You MUST drag the assets folder in. (This is
     why an upload can end up with wardens but no assets folder.)
     wardens must end up sitting NEXT TO the assets/ folder.
  4. Type a short message and click "Commit changes".
  5. Settings > Pages > deploy from your main branch. Your book is live at
     https://<you>.github.io/<repo>/wardens

HOW RETRIEVAL WORKS
  The reader fetches each track/illustration ONLY when the reader reaches it
  (lazy), by its stable path under assets/. Nothing loads up front, so audio
  bandwidth stays low and the first page opens instantly.

NOTE: reader comments & analytics need the optional Supabase step — see the
project spec. Without it, the book reads & plays perfectly; discussion is local-only.