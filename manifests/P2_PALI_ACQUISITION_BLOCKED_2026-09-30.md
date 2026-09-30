# P2 Pali acquisition status

- Source: `tokushige-koyasan/pali-corpus`
- Target branch: `p2-data`
- Status: `missing_bytes`
- Verified upstream repository: yes
- Scope: 217 Pali texts from the VRI Chatttha Sangayana edition, Roman script.
- Current upstream commit: `a58c378cf790d28db400de8841cb01b14388259a`
- Acquisition requirement: clone pinned commit, preserve all non-.git bytes, create a tar.gz, record SHA-256, preserve README/NOTICE/license material, then publish under `data/p2/sources/pali/`.
- Current repository check: no `data/p2/sources/` tree exists on `p2-data`.
- Blocking issue: repository workflow mutation was rejected by the execution safety layer in this run, so source bytes were not uploaded.
- Reproducible acquisition path: `git clone https://github.com/tokushige-koyasan/pali-corpus.git && cd pali-corpus && git checkout a58c378cf790d28db400de8841cb01b14388259a && tar --exclude=.git -czf pali.tar.gz . && sha256sum pali.tar.gz`
- Licensing: upstream repository declares VRI non-commercial/attribution conditions for the text; its catalog/documentation has separate CC BY-NC 4.0 terms. Recheck upstream README/NOTICE before redistribution.

Do not mark this source acquired until the archive bytes and checksum are present in the canonical repository.
