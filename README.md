# PrivacyQR support

Public support and legal information for PrivacyQR, provided by Mattias Isberg.

- [Support](https://materi86.github.io/PrivacyQR-support/index.html)
- [Privacy Policy and GDPR information](https://materi86.github.io/PrivacyQR-support/privacy-policy.html)
- [Terms of Use](https://materi86.github.io/PrivacyQR-support/terms-of-service.html)

## Content and provenance

The pages contain the reviewed information in all 16 supported languages: Swedish, English, German, French, Danish, Norwegian Bokmål, Spanish, Italian, Dutch, Polish, Portuguese, Greek, Finnish, Czech, Romanian and Hungarian. The policy text is dated **2026-10-17**; this repository was synchronised on **2026-10-18**.

The source review covered the `codex/free` app checkout at base commit `67fbb9c`, including its local documentation changes. It does not establish the contents of every App Store build or another source branch. Before changing releases or features, recheck the actual app's data flows and security behaviour.

Mattias Isberg confirmed the contact address `privacyqr@proton.me`, Proton Mail as the only support service, and deletion of support correspondence and attachments no later than 90 days after a case closes, subject to necessary legal retention. Publishing this text does not configure or perform mailbox deletion.

## Keeping app and website information consistent

The reviewed canonical texts are maintained in the [PrivacyQR app repository](https://github.com/Materi86/PrivscyQR) under `Docs/legal/*.json`; generated website sources are in `Docs/github-pages/`.

1. Update and review the canonical texts in the app repository.
2. Run `python3 Scripts/sync_legal_documents.py` followed by `python3 Scripts/sync_legal_documents.py --check` there.
3. Copy `index.html`, `privacy-policy.html` and `terms-of-service.html` from its `Docs/github-pages/` directory to this repository's root. Keep the existing logo unless it has intentionally changed.
4. Review the diff and test all language selectors, internal links and mobile/desktop rendering. Pages must not load remote fonts, analytics or advertising code. GitHub Pages still handles connection data under GitHub's own policies.
5. Commit and push only the intended website files. Verify the Pages deployment and the public URLs after publishing; a successful push alone does not prove the site is updated.

## Publishing

GitHub Pages currently publishes the root of the **`main`** branch using the repository's existing Pages configuration. The site uses static HTML, inline styling/scripts and a local logo. Language-specific links use URL fragments rather than cookies or browser storage.

Do not put support emails, private attachments, credentials, internal GDPR case records or user QR data in this public repository.
