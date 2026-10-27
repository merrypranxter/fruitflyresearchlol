# Original PDF preservation — pending binary upload

The four original user-supplied PDF **binary files are not stored in this repository yet**. The GitHub connector used to initialize this vault supports UTF-8 text and Git blobs, but it did not have access to the uploaded PDFs' raw bytes in this operation. We therefore committed full searchable text transcriptions, explicitly marked as such.

**Do not claim the PDFs are in GitHub merely because their extracted words are.**

Once uploaded through GitHub or a Git-capable local client, retain these originals here with exact filenames:

- `Connectome Artificial Life Exploration.pdf` (R01; 26 pages; 542615 bytes)
- `The Unlimited Body_ Everything a Simulated Fly Brain Could Possibly Control.pdf` (R02; 30 pages; 210158 bytes)
- `The Unlimited Body.pdf` (R03; 48 pages; 2237511 bytes)
- `I feel like u cut off and coulda kept going so her.pdf` (R04; 44 pages; 1622306 bytes; continuation of R03)

Use [manifest.json](../manifest.json) SHA-256 digests to verify exact byte identity. Original PDFs contain formatted tables, page images, equations and layouts that text transcription may lose.

Once the binary files are actually uploaded and checked, change their manifest `github_pdf_status` to `committed` and update this note and README. Until then, source PDF binary status remains **PENDING**.
